# GUÍA PARA COMPLETAR FORMULARIO — PROYECTO CERRADO

**Uso interno Elitsoft**

---

## ¿Cuándo usar este modelo?

✅ **Usar PROYECTO CERRADO cuando:**
- Cliente tiene requerimiento **100% claro**
- Se necesita **precio fijo** (fixed price)
- El alcance debe estar **cerrado y firmado**
- Cliente necesita "entregar ON DATE"
- Modelo: Fixed scope, Fixed price, Fixed timeline

❌ **NO usar cuando:**
- Cliente "no está seguro de lo que necesita" → hacer DIAGNÓSTICO primero
- Hay mucha incertidumbre → usar SERVICIO ÁGIL
- Son recursos/HH puro → usar OUTSOURCING

---

## Consejos por sección

### FICHA EJECUTIVA

- Llena al FINAL
- El entregable principal es LO que se entrega
- Presupuesto: suma HH × tarifa (sin margen de error)

---

### 1-2. OBJETIVO Y PROBLEMA

**Preguntas:**
- "¿Qué es lo que necesitan EXACTAMENTE?" (una frase, no un párrafo)
- "¿Qué impacto tiene NO tenerlo?" (datos de negocio)
- "¿Hay una fecha límite?"

**Rojo de alerta:**
- Si dice "no sabemos exactamente" → NO proceder
- Si hay incertidumbre en tech → NO proceder

---

### 3. ALCANCE (CRÍTICO)

**Este es donde fijas límites.**

**INCLUDE:**
- Enumera TODO lo que hace el sistema
- Enumera TODO lo que se entrega (doc + código + etc)

**EXCLUDE:**
- Migración de datos históricos (si no es explícito)
- Capacitación masiva (si no es explícito)
- Mantenimiento post-go-live
- Cambios post-proyecto
- Infraestructura/servidores (si el cliente debe pagar)

**Ej. bueno de exclusión:**
```
NO INCLUYE:
- Capacitación a usuarios (es responsabilidad del cliente)
- Mantenimiento de infraestructura
- BI/Reportes avanzados
- Integración con sistemas no mencionados
```

---

### 4-5. AS-IS Y TO-BE

**AS-IS:** describe EL DÍA DE HOY (bien detallado)
**TO-BE:** describe DESPUÉS (qué cambia, no cómo)

**Preguntas:**
- "Hoy, paso a paso: ¿Quién toca qué?"
- "Cómo quieren que sea: describe un día típico"
- "¿Qué desaparece, qué aparece?"

---

### 6. REQUERIMIENTOS (EXHAUSTIVO)

**RF (Requerimientos Funcionales):**
- "El sistema DEBE permitir..."
- "El usuario PUEDE hacer..."
- Enumera cada función de negocio

**RT (Requerimientos Técnicos):**
- Performance: respuesta en <2 segundos
- Disponibilidad: 99.5% uptime
- Seguridad: encriptación de datos sensibles
- Escalabilidad: crecer sin rediseño

**Preguntas críticas:**
- "¿Cuántos usuarios simultáneos?"
- "¿Cuántas transacciones por segundo?"
- "¿Necesita estar disponible 24x7 o solo 8x5?"
- "¿Datos sensibles?"

**Tipificación:**
- RF vs RT vs RNF (no-functional)
- Cada una tiene criterio de aceptación

---

### 7. ESPECIFICACIÓN DETALLADA

**Aquí es donde el consultor debe profundizar MUCHO.**

Para cada funcionalidad:
- ¿Quién toca?
- ¿Qué hace exactamente?
- ¿Qué valida el sistema?
- ¿Cuál es el output?
- ¿Qué pasa si falla?

**Ej:**
```
CREAR FACTURA:
1. Usuario selecciona cliente
2. Sistema valida cliente existe + sin deuda
3. Usuario ingresa ítems (N items)
4. Sistema calcula subtotal + impuestos
5. Usuario confirma pago
6. Sistema crear archivo PDF + envía mail
7. Sistema registra en BD
```

---

### 8. ARQUITECTURA

**Preguntas:**
- "¿Cuántas capas?" (frontend, backend, bd)
- "¿De dónde vienen los datos?" (sistemas externos)
- "¿Dónde se guardan?"
- "¿Quién accede a qué?" (front-office, back-office, API)

**Stack:**
- No inventes. Pregunta qué usa el cliente.
- Si es greenfield: sugiere stack moderno pero justifica

---

### 9. DATOS Y MIGRACIÓN

**Si hay migración:**
- ¿De dónde?
- ¿Cuántos registros?
- ¿Qué validaciones?
- ¿Data cleanup necesario?

**Si NO hay migración:**
- Excluir esta sección

---

### 10. SEGURIDAD

**Preguntas:**
- "¿Qué datos son sensibles?" (PII, financiero, etc)
- "¿Acceso por rol?" 
- "¿Necesita audit trail?"
- "¿Regulaciones?" (GDPR, SOX, etc)
- "¿Penetration testing?"

---

### 11. CRITERIOS DE ACEPTACIÓN

**Aquí pones las "checkboxes" finales.**

Funcional:
- RF1 ✓
- RF2 ✓
- Integraciones ✓
- Performance ✓

Técnico:
- Tests 80%+
- Documentación
- Runbooks

Seguridad:
- Pen test pasado
- Validación compliance

---

### 12. PLAN DE TRABAJO

**Típico: 9-10 semanas**

**Fases:**
1. Análisis + Diseño (2 sem)
2. Desarrollo (4 sem)
3. QA (2 sem)
4. UAT + Go-live (1 sem)

**Hitos:** Son los puntos de control → aprobación cliente

---

### 14. DIMENSIONAMIENTO

**Cálculo honesto:**
- Tech Lead: 30-50% (todo el proyecto)
- Backend Dev: 100% (8-9 semanas)
- Frontend Dev: 100% (7-8 semanas)
- QA: 100% (3-4 semanas)
- PM: 20% (todo el proyecto)

**Total típico: 250-400 HH** (depende complejidad)

**Fórmula:**
- Baja complejidad: 250 HH
- Complejidad media: 300-350 HH
- Alta complejidad: 400+ HH

---

### 15. MODELO ECONÓMICO

**CRÍTICO: Esto es FIXED PRICE**

**Cálculo:**
- Total HH × Tarifa promedio = Subtotal
- Agrega: Licencias, infraestructura (si es tu responsabilidad)
- Agrega: Contingency reserve (5-10% INTERNO, no pases al cliente)
- Total = Presupuesto final

**Estructura de pago sugerida:**
- 30% Anticipo
- 20% Hito Diseño
- 30% Hito Dev completado
- 20% Go-live

**Riesgo:** Si subestimas, es tu problema. SEE CONSERVATIVE.

---

### 16. RIESGOS

**Riesgos típicos:**
- Legacy complexity mayor a lo esperado
- Datos quality peor
- Cambios mid-project
- Integración más compleja
- Accesos tardíos

**Para cada riesgo:**
- Probabilidad (Alta/Media/Baja)
- Impacto (Alto/Medio/Bajo)
- Qué haces si ocurre

---

### 17-20. SUPUESTOS / EXCLUSIONES / DEPENDENCIAS

**SUPUESTOS** (cosas que deben ocurrir):
- "Cliente proporciona acceso en día 1"
- "Documentación técnica disponible"
- "Cambios máximo 2 durante proyecto (resto = adicionales)"

**EXCLUSIONES** (lo que NO haces):
- "No incluye capacitación masiva"
- "No incluye mantenimiento post-go-live"

**DEPENDENCIAS:**
- Qué necesitas del cliente
- Qué necesitas externo

---

## Checklist ANTES de entregar formulario

- ☐ ¿Objetivo está en UNA frase y es claro?
- ☐ ¿AS-IS está bien documentado?
- ☐ ¿TO-BE es diferente y claro del AS-IS?
- ☐ ¿Todas las RF tienen criterios de aceptación?
- ☐ ¿RTs tienen métricas específicas?
- ☐ ¿Alcance tiene mínimo 5 INCLUDES y 5 EXCLUDES?
- ☐ ¿Horas tienen lógica?
- ☐ ¿Hay documentación de cliente sobre current state?
- ☐ ¿Hay riesgos REALES (no obvios)?
- ☐ ¿Cliente firmó alcance?

---

## Red flags absolutos

❌ Cliente dice: "No sabemos exactamente qué necesitamos"  
❌ Cliente dice: "Luego le pedimos cambios"  
❌ Cliente dice: "¿Cuánto cuesta aproximadamente?"  
❌ No hay stakeholder técnico del cliente  
❌ No hay acceso a documentación legacy  

**Si hay red flags: SUGIERE DIAGNÓSTICO PRIMERO**

---

## Próximo paso

Una vez completado este formulario → pasar a **prompt_generador.md** para generar el documento técnico formal
