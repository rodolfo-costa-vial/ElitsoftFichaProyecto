# ANÁLISIS DE COSTOS — PROYECTO CERRADO
**Documento de presupuesto detallado y márgenes**

---

## 💰 RESUMEN EJECUTIVO

| Concepto | Valor |
|----------|-------|
| **Cliente** | [CLIENTE] |
| **Proyecto** | [NOMBRE] |
| **Duración** | [SEMANAS] semanas |
| **Equipo** | [N] personas |
| **Costo Proyecto** | [COSTO] USD |
| **Venta Proyecto** | **[VENTA] USD** |
| **Margen** | **[%]** |

---

## 1. EQUIPO Y PERSONAS

### Recursos Humanos

| Rol | Seniority | HH | Tarifa | Subtotal |
|-----|-----------|-----|--------|----------|
| Tech Lead | Sénior | [HH] | [USD/HH] | [SUB] |
| Backend Dev | Semi-Sénior | [HH] | [USD/HH] | [SUB] |
| Backend Dev | Semi-Sénior | [HH] | [USD/HH] | [SUB] |
| Frontend Dev | Semi-Sénior | [HH] | [USD/HH] | [SUB] |
| QA Lead | Semi-Sénior | [HH] | [USD/HH] | [SUB] |
| QA Junior | Junior | [HH] | [USD/HH] | [SUB] |
| DevOps | Semi-Sénior | [HH] | [USD/HH] | [SUB] |
| PM | Sénior | [HH] | [USD/HH] | [SUB] |
| **TOTAL RH** | | **[HH]** | | **[TOTAL_RH]** |

### Distribución por Fase

```
Fase 1 (Análisis): [HH] → [%] del total
Fase 2 (Dev):      [HH] → [%] del total
Fase 3 (QA):       [HH] → [%] del total
Fase 4 (Go-Live):  [HH] → [%] del total
```

---

## 2. COSTOS DE INFRAESTRUCTURA

| Item | Costo/Mes | Meses | Subtotal |
|------|-----------|-------|----------|
| Hosting DEV | [COSTO] | [N] | [SUB] |
| Hosting STAGING | [COSTO] | [N] | [SUB] |
| Hosting PROD | [COSTO] | [N] | [SUB] |
| Licencias | [COSTO] | 1 | [SUB] |
| CDN | [COSTO] | [N] | [SUB] |
| Monitoreo | [COSTO] | [N] | [SUB] |
| **TOTAL INFRA** | | | **[TOTAL_INFRA]** |

---

## 3. PRESUPUESTO TOTAL COSTO

```
Recursos Humanos        [TOTAL_RH]
Infraestructura         [TOTAL_INFRA]
                        ─────────────
Subtotal Costo          [SUBTOTAL_COSTO]
Contingencia Interna (%) [CONTINGENCIA]
                        ═════════════════
COSTO TOTAL PROYECTO    [COSTO_TOTAL]
```

---

## 4. PRESUPUESTO VENTA (FIXED PRICE)

```
Costo Proyecto          [COSTO_TOTAL]
Margen Deseado (%)      [MARGEN_%]
                        ─────────────
Subtotal Venta          [SUBTOTAL_VENTA]
IVA (19%)               [IVA]
                        ═════════════════
TOTAL VENTA AL CLIENTE  [TOTAL_VENTA]
```

---

## 5. ESTRUCTURA DE PAGO

| Hito | % | Monto | Disparo |
|------|-----|-------|---------|
| Anticipo | 30% | [MONTO] | Al firmar |
| Hito 1: Diseño | 20% | [MONTO] | Aprobación diseño |
| Hito 2: MVP | 30% | [MONTO] | MVP testeado |
| Hito 3: Go-Live | 20% | [MONTO] | En producción |
| **TOTAL** | **100%** | **[TOTAL_VENTA]** | |

---

## 6. ANÁLISIS DE RENTABILIDAD

### Márgenes

| Métrica | Valor |
|---------|-------|
| Costo Total | [COSTO] USD |
| Venta Total | [VENTA] USD |
| Margen Absoluto | [MARGEN] USD |
| Margen % | [%] |
| **Margen/HH** | **[USD/HH]** |

### Validación

| Validación | Valor | Status |
|-----------|-------|--------|
| Margen mín. 30% | [%] | ✅/❌ |
| ROI positivo | [%] | ✅/❌ |
| Costo/HH <$60 | [USD/HH] | ✅/❌ |

---

## 7. ESCENARIOS DE RIESGO

### Pesimista: -15% Productivity
```
HH reales:  [HH_AUMENTO]
Margen:     [MARGEN_%]
```

### Base: 100%
```
HH:         [HH]
Margen:     [MARGEN_%]
```

### Optimista: +10% Efficiency
```
HH reales:  [HH_DISMINUCION]
Margen:     [MARGEN_%]
```

---

## 8. FACTORES DE RIESGO FINANCIERO

| Riesgo | Impacto | Probabilidad | Mitigación |
|--------|---------|-------------|-----------|
| Alcance crece | -$[MONTO] | [PROB] | Control cambios |
| Plazo extiende | -$[MONTO] | [PROB] | Hitos + PenaltyAct |
| Infra más cara | -$[MONTO] | [PROB] | Reserved contingency |
| Turnover equipo | -$[MONTO] | [PROB] | Knowledge transfer |

---

## 9. APROBACIÓN COMERCIAL

| Rol | Nombre | OK | Notas |
|-----|--------|-----|-------|
| CFO/Finance | [NOMBRE] | ☐ | |
| Sales Lead | [NOMBRE] | ☐ | |
| Tech Lead | [NOMBRE] | ☐ | |

---

**Documento generado:** [FECHA_HOY]  
**Vigencia:** [DÍAS] días
