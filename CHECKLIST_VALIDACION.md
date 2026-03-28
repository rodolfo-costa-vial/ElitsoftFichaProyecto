# CHECKLIST DE VALIDACIÓN — PRE-GENERACIÓN DE DOCUMENTOS

**Antes de pasar formulario a IA, verifica que cumpla este checklist**

---

## 🎯 CHECKLIST GENERAL (TODOS LOS TIPOS)

### A. Información del Cliente
- [ ] Nombre cliente completo
- [ ] Área solicitante identificada
- [ ] Contacto principal nombrado (email + teléfono)
- [ ] Fecha del levantamiento registrada
- [ ] Consultor/PM asignado

### B. Contexto del Proyecto
- [ ] Objetivo/problema del cliente descrito
- [ ] Industry/tamaño del cliente documentado
- [ ] Situación actual (AS-IS) explicada
- [ ] Visión objetivo (TO-BE) clara
- [ ] Impacto negativo actual cuantificado (si posible)

### C. Integridad de Datos
- [ ] <30% de campos vacíos (máximo tolerable)
- [ ] Sin errores ortográficos obvios
- [ ] Números tienen coherencia lógica (ej: HH > 0, tarifa > 0)
- [ ] No hay datos contradictorios

---

## 📋 CHECKLIST ESPECÍFICO — OUTSOURCING

### Levantamiento
- [ ] Seniority del recurso claro (Junior/Semi/Senior/Lead)
- [ ] Stack tecnológico específico (no solo "developer")
- [ ] Horas/semana definidas (mín. 20, máx. 40)
- [ ] Duración en meses especificada
- [ ] SLA o nivel de disponibilidad definido
- [ ] Modalidad trabajo claro (remoto/presencial/híbrido)
- [ ] Riesgos mín. 2 identificados
- [ ] Supuestos mín. 2 documentados

### Artefactos
- [ ] Componentes a tocar/mantener enumerados
- [ ] Especificaciones por componente presente
- [ ] DoD para el recurso definido

### Costos
- [ ] Tarifa USD/HH documentada
- [ ] Cálculo simple HH × Tarifa presente
- [ ] Contingencia considerada (% o USD)
- [ ] Margen bruto analizado

---

## 📋 CHECKLIST ESPECÍFICO — SERVICIO ÁGIL

### Levantamiento
- [ ] AS-IS documentado en detalle (cómo es HOY)
- [ ] TO-BE claro (cómo será DESPUÉS)
- [ ] Mínimo 5 RF especificados
- [ ] Mínimo 3 RT especificados
- [ ] RF con criticidad (Must/Should/Could)
- [ ] Integraciones identificadas
- [ ] Riesgos mín. 3 documentados
- [ ] Supuestos mín. 3 documentados
- [ ] Plazo estimado en semanas

### Artefactos
- [ ] Artefactos por fase enumerados
- [ ] DoD (Definition of Done) para cada artefacto
- [ ] Quality gates definidos (test coverage, security, etc)

### Costos
- [ ] Equipo y roles identificados
- [ ] HH por rol estimadas
- [ ] Tarifas por seniority presentes
- [ ] Costos infra por mes documentados
- [ ] Contingencia incluida
- [ ] Estructura pago en 3-4 cuotas

---

## 📋 CHECKLIST ESPECÍFICO — PROYECTO CERRADO

### Levantamiento
- [ ] Objetivo en UNA frase clara
- [ ] Problema cuantificado (ej: "hoy toma 6 hrs, queremos 2 hrs")
- [ ] INCLUDES mín. 5 items específicos
- [ ] EXCLUDES mín. 5 items específicos
- [ ] Mínimo 8 RF detallados
- [ ] Mínimo 5 RT técnicos
- [ ] Criterios aceptación por RF definidos
- [ ] Hitos en semanas especificados
- [ ] Riesgos mín. 4 documentados
- [ ] Supuestos mín. 4 documentados
- [ ] Dependencias cliente identificadas

### Artefactos
- [ ] Inventario EXHAUSTIVO de componentes
- [ ] Cada artefacto con especificación técnica
- [ ] DoD checklist por artefacto
- [ ] Hitos de validación con criterios
- [ ] Matriz de recursos por artefacto

### Costos
- [ ] Equipo completo listado (Tech Lead, Devs, QA, PM, etc)
- [ ] HH realista por rol/fase
- [ ] Tarifas internas (costo para Elitsoft)
- [ ] Costos infra desglosados (Dev/Staging/Prod)
- [ ] Contingencia interna documentada
- [ ] Margen objetivo establecido (típico 40%)
- [ ] Estructura pago 30-20-30-20 definida
- [ ] IVA incluido en cálculo final

---

## ⚠️ RED FLAGS — RECHAZA SI VES ESTO

- [ ] "No sabemos exactamente qué necesitamos" → Sugiere diagnóstico
- [ ] Margen <20% → Demasiado ajustado, riesgo alto
- [ ] Margen >60% → Probablemente sobreprecio, revisar
- [ ] HH estimadas >1000 → Probablemente subestimado scope
- [ ] HH estimadas <50 → Probablemente sobrestimado scope
- [ ] No hay contacto cliente identificado
- [ ] Plazo = 1 semana → Poco realista (excepto bugfixes)
- [ ] Plazo = 6+ meses sin hitos intermedios
- [ ] Alcance totalmente vago ("hacer un app")
- [ ] Cliente pide "luego le pedimos cambios"
- [ ] Documentación legacy no disponible/accesible

---

## ✅ CRITERIOS DE APROBACIÓN

**Mínimo requerido para pasar a IA:**

- [ ] Información cliente: 100% (nombre, contacto, contexto)
- [ ] Contexto del proyecto: 90%+ completitud
- [ ] Campos específicos del levantamiento: 80%+ completitud
- [ ] Riesgos y supuestos: documentados
- [ ] Sin red flags críticos

**Si cumple:** Genera documento  
**Si no cumple:** Vuelve con cliente, solicita información

---

## 📊 Scoring

Cuenta checkboxes completados:

- **0-20%:** ❌ Rechazar, muy incompleto
- **20-50%:** 🟡 Revisar con cliente, faltan datos críticos
- **50-80%:** 🟡 Depende, aceptable si no hay red flags
- **80-100%:** ✅ Listo para generar documento

---

## Uso Rápido

```
1. Abre formulario completado
2. Ejecuta checklist correspondiente a su tipo
3. Cuenta ✅
4. Si score >80% y sin red flags → GENERA
5. Si score <80% o hay red flags → RECHAZA + feedback al consultor
```

---

**Última actualización:** 27-03-2026  
**Versión:** 1.0
