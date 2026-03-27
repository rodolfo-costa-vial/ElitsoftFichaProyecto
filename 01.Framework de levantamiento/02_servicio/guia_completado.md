# GUÍA PARA COMPLETAR FORMULARIO — SERVICIO ÁGIL

**Uso interno Elitsoft**

---

## ¿Cuándo usar este modelo?

✅ **Usar SERVICIO ÁGIL cuando:**
- Cliente tiene una **idea general** del problema
- El alcance puede **evolucionar** durante el proyecto
- Se trabajará por **fases incrementales** 
- Habrá **entregas parciales** testables
- Modelo: Por proyecto (precio fijo) pero con flexibilidad

❌ **NO usar cuando:**
- Cliente tiene requerimiento 100% claro → usar PROYECTO cerrado
- Son solo horas/recursos → usar OUTSOURCING
- No hay presupuesto definido → hacer diagnóstico primero

---

## Consejos por sección

### FICHA EJECUTIVA
- Llena al FINAL del levantamiento
- El "problema clave" es lo que sintetiza TODO
- Inversión: suma de HH × tarifa

### 1. CONTEXTO GENERAL

**Preguntas clave:**
- "¿Cuál es el problema #1 que quieren resolver?"
- "¿Cómo lo están viviendo HOY?" (efecto práctico)
- "¿Quién más se verá beneficiado internamente?"

**Red flags:**
- Si dicen "tenemos varias prioridades" → profundizar en la #1
- Si hay conflicto de criterios → documento explícitamente como RIESGO

---

### 2. SITUACIÓN ACTUAL (AS-IS)

**Este es el corazón.**

**¿Qué preguntar?**
- "Describe un día típico: ¿Cómo fluye la información?"
- "¿Dónde se detiene o complica el proceso?"
- "¿Quién toca esto? ¿Cuántas personas?"
- "¿Cuántos datos procesamos por día?"

**Cómo documentar:**
- Menciona el sistema usado (legacy, ERP, etc.)
- Menciona tiempo que demora (ej: "toma 4 horas consolidar")
- Menciona personas involucradas (áreas)

**Ej. bueno:**
```
Hoy el equipo de facturación (5 personas) exporta datos de SAP a Excel,
limpia el archivo (3 horas), lo valida contra un sheet maestro (2 horas),
y carga a legacy billing system (1 hora). Total proceso: 6 horas/día.
```

**Ej. malo:**
```
El proceso es manual y está automatización sea posible.
```

---

### 3. VISIÓN OBJETIVO (TO-BE)

**Preguntas:**
- "¿Cómo se vería si esto estuviera AUTOMATIZADO?"
- "¿Qué pasos desaparecerían?"
- "¿En cuánto tiempo?"
- "¿Quién estaría haciendo qué?"

**Tip:** No preguntes por solución técnica, pregunta por el estado deseado.

---

### 4. REQUERIMIENTOS

**Requiere más profundidad que outsourcing o diagnostico.**

**Preguntas:**
- "¿Cuál es el dato que SIEMPRE debe estar?" (obligatorio)
- "¿Cuál es el dato que 'sería lindo' tener?" (nice-to-have)
- "¿Quién valida esto?" (criterio de aceptación)

**Tipificación (MoSCoW):**
- **Must:** Sin esto no funciona
- **Should:** Hace el sistema útil
- **Could:** "Nice to have" pero no es crítico

---

### 5. ARQUITECTURA PROPUESTA

**Preguntas:**
- "¿Quiénes son los usuarios finales?" (backend office, public web, mobile?)
- "¿De dónde vienen los datos?" (SAP, Oracle, APIs?)
- "¿Dónde se guardan?" (cloud, on-prem, hybrid?)
- "¿Necesita reportes?"
- "¿Notificaciones?"

**Restricciones:**
- "¿Restricciones de seguridad por industria?" (finanzas = muy estricto)
- "¿Performance: cuántas transacciones/segundo?"
- "¿Disponibilidad: 24x7 o 8x5?"

---

### 6. INTEGRACIONES

**Preguntas clave:**
- "¿Con qué sistemas hablará?" (SAP, Oracle, legacy?)
- "¿Ya existen APIs o hacemos custom?"
- "¿Frecuencia?" (real-time, batch diario, semanal?)
- "¿Volumen?" (10 registros/día o 100k?)

**Complejidad típica:**
- APIs modernas (REST, GraphQL) = Low complexity
- SOAP/Web Services antiguo = Medium
- File dumps / EDI = High

---

### 7. SEGURIDAD

**Preguntas:**
- "¿Cuáles datos son sensibles?" (PII, financiero, etc.)
- "¿Quiénes deben tener acceso?" (roles)
- "¿Necesitan auditoría?" (trazabilidad de cambios)
- "¿Regulaciones?" (GDPR, SOX, HIPAA, etc.)

---

### 8. IA (si aplica)

**Preguntas si mencionó "AI", "predicción", "clasificación":**
- "¿Quiénes son los expertos internos que pueden facilitar datos históricos?"
- "¿Cuántos registros tienen para entrenar?" (mínimo 1000-5000 según caso)
- "¿Cada cuánto necesita reentrenamiento?"

**Si NO menciona IA:**
- Déjalo en BLANCO, no inventes

---

### 9. PLAN DE TRABAJO

**Típico para servicio ágil: 9-12 semanas**

**Fases sugeridas:**
1. Análisis + Diseño (1-2 semanas)
2. Sprint 1-2 desarrollo (3-4 semanas)
3. QA + Ajustes (1-2 semanas)
4. Go-live + Capacitación (1 semana)

**Preguntas:**
- "¿Hay alguna fecha crítica?" (año nuevo, auditoría, etc.)
- "¿Quién del cliente estará dedicado?"

---

### 10. DIMENSIONAMIENTO

**Cálculo típico:**
- Tech Lead sénior: 40-50% dedicación todo el proyecto
- 2 devs: 100% durante fases 2-3, reducen en 4
- 1 QA: último mes 100%, luego ramp down

**Fórmula:**
- Análisis: 40-60 HH
- Backend: 120-200 HH (según complejidad)
- Frontend: 60-100 HH
- QA: 40-60 HH
- Gestión: 20% del total

**Total típico: 300-500 HH** (9-12 semanas con 4-5 personas)

---

### 11. MODELO ECONÓMICO

**Importante: NO hagas precio fijo si el cliente cambia requerimientos cada semana.**

**Preguntas:**
- "¿Hay presupuesto flexible o es fijo?"
- "¿Cambios durante proyecto se cobran extra o están inclusos?"

**Estructura recomendada:**
- Horas reservadas para cambios (ej: 5%)
- Cambios beyond = son adicionales
- Esto lo documentas en SUPUESTOS

---

### 12. RIESGOS

**Riesgos típicos de servicios ágil:**
- Alcance creep (cliente pide más)
- Datos legacy son peor de lo esperado
- Accesos lentos en cliente
- Cambios de prioridad mid-project
- Sistema legacy complejo para integración

**Para cada riesgo:**
- ¿Probabilidad? (Alta/Media/Baja)
- ¿Impacto? (Alto/Medio/Bajo)
- ¿Cómo mitigo?

---

### 13. SUPUESTOS

**Típicos:**
- "Cliente proporciona acceso a todos los sistemas en día 1"
- "Cambios de requerimiento limitados a [N] por fase"
- "Datos legacy están en [formato, ubicación]"
- "Contraparte dedicada 8 horas/semana"

---

### 14. EXCLUSIONES

**Típicas:**
- "No incluye migración de datos históricos"
- "No incluye capacitación a usuarios finales (solo IT)"
- "No incluye mantenimiento post-go-live"
- "No incluye infraestructura/servers"

---

## Checklist antes de entregar

- ☐ ¿Tiene AS-IS bien documentado?
- ☐ ¿Tiene TO-BE claro?
- ☐ ¿MoSCoW está priorizado?
- ☐ ¿Las horas tienen lógica?
- ☐ ¿Hay al menos 3 riesgos reales?
- ☐ ¿Cliente validó alcance?
- ☐ ¿Hay fecha crítica mencionada?

---

## Próximo paso

Una vez completado este formulario → pasar a **prompt_generador.md** para generar el documento técnico formal
