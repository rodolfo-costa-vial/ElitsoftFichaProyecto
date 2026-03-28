# MATRIZ DE TRAZABILIDAD — REQUERIMIENTO → ARTEFACTO → COSTO

**Mapeo de requerimientos a componentes técnicos a líneas de presupuesto**

---

## ¿Para Qué Sirve?

Garantizar que:
- ✅ Todo requerimiento tiene un artefacto técnico que lo implementa
- ✅ Todo artefacto tiene línea de costo presupuestada
- ✅ No hay "huecos" donde se cae algo
- ✅ Control de scope y presupuesto centralizado

---

## Uso

### Paso 1: Extrae IDs del Levantamiento

Del documento de requerimientos, obtén:
```
RF-001: [Descripción requerimiento]
RF-002: [Descripción requerimiento]
RT-001: [Descripción técnico]
```

### Paso 2: Extrae Artefactos

Del documento de artefactos:
```
ARTEFACTO-001-Backend-API: [Descripción]
ARTEFACTO-002-Frontend-Screen: [Descripción]
ARTEFACTO-003-Database-Schema: [Descripción]
```

### Paso 3: Mapea a Líneas de Costo

Del documento de costos:
```
Costo-RH-Backend: [HH] × [USD/HH] = [Monto]
Costo-RH-Frontend: [HH] × [USD/HH] = [Monto]
Costo-Infra-DB: [Monto/mes] × [Meses]
```

### Paso 4: Rellena Matriz

| RF ID | Requerimiento | Artefacto ID | Artefacto Descripción | Línea Costo | Monto USD | Status |
|-------|---------------|--------------|----------------------|-------------|----------|--------|
| RF-001 | [desc] | ARTEFACTO-001 | [desc] | Costo-RH-Backend | [monto] | ✅ |
| RF-002 | [desc] | ARTEFACTO-002 | [desc] | Costo-RH-Frontend | [monto] | ✅ |
| RT-001 | [desc] | ARTEFACTO-003 | [desc] | Costo-Infra-DB | [monto] | ✅ |

---

## Análisis Derivado

### Coverage
```
Total RF: [N]
RF con artefacto: [N]
Coverage %: [%]

Si <100% → ⚠️ Hay requerimientos sin implementación definida
```

### Completitud de Costos
```
Total Artefactos: [N]
Artefactos con costo: [N]
Completitud %: [%]

Si <100% → ⚠️ Hay artefactos sin línea de presupuesto
```

### Validación de Scope
```
¿Artefactos en documento de requerimientos coinciden con artefactos en documento técnico?
✅ SÍ → Scope alineado
❌ NO → Scope DRIFT → Action required
```

---

## Plantilla Completa

```markdown
# MATRIZ DE TRAZABILIDAD — [CLIENTE] [PROYECTO]

**Fecha:** [FECHA]  
**Versión:** v1.0  
**Estado:** [Draft / Final / Signed-off]

---

## 1. COBERTURA GENERAL

| Métrica | Valor | Status |
|---------|-------|--------|
| Total Requerimientos | [N] | |
| Requerimientos mapeados | [N] | ✅/⚠️ |
| Total Artefactos | [N] | |
| Artefactos costeados | [N] | ✅/⚠️ |
| Presupuesto total | [USD] | |

---

## 2. MATRIZ DETALLADA

| RF/RT ID | Descripción | Artefacto(s) | Línea Costo | Monto | Responsable | Status |
|----------|-------------|--------------|-------------|-------|-------------|--------|
| RF-001 | [desc] | ART-001 | COS-Backend-001 | [USD] | [persona] | ✅ |
| RF-002 | [desc] | ART-002 | COS-Frontend-001 | [USD] | [persona] | ✅ |
| [...] | | | | | | |

---

## 3. GAPS IDENTIFICADOS

### Requerimientos sin Artefacto
- [RF-X]: [Descripción] → Acción: [QUÉ HACER]

### Artefactos sin Costo
- [ART-X]: [Descripción] → Acción: [QUÉ HACER]

---

## 4. VALIDACIÓN DE SCOPE

✅ Todos RF tienen artefacto  
✅ Todos artefactos tienen costo  
✅ Presupuesto totales coinciden  
❌ [Si hay problema]: Describir

---

## 5. RECOMENDACIONES

- [Recomendación 1]
- [Recomendación 2]

---

## 6. SIGN-OFF

| Rol | Nombre | Revisión | Aprobación |
|-----|--------|----------|-----------|
| Tech Lead | [NOMBRE] | [FECHA] | ☑ |
| Project Manager | [NOMBRE] | [FECHA] | ☑ |
| CFO/Finance | [NOMBRE] | [FECHA] | ☑ |

**Documento preparado por:** [NOMBRE]  
**Fecha:** [FECHA]  
**Vigencia:** [DÍAS] días
```

---

## Uso Práctico

**Escenario:** Cliente pide cambio mid-project

→ Consulta matriz  
→ ¿El cambio afecta algún RF?  
→ ¿Ese RF tiene artefacto?  
→ ¿Ese artefacto tiene costo?  
→ Calcula impact en presupuesto  
→ Notifica cliente con líneas específicas de costo que cambian

---

**Última actualización:** 27-03-2026
