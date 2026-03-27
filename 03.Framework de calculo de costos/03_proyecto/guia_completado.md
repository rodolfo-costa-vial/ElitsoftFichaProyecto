# GUÍA — CÁLCULO DE COSTOS (PROYECTO CERRADO)

**Uso interno Elitsoft**

---

## ¿Qué Es?

Documento que calcula **costo total** (HH + infra) y **precio de venta** (fixed price con margen), para proyecto cerrado.

---

## Cómo Completar

### 1. EQUIPO Y HH

**Pregunta:** "¿Quiénes trabajan y cuántas horas cada uno?"

Tabula:
- Tech Lead (Sénior): 10 semanas × 30% = 120 HH
- Backend (Semi): 8 semanas × 100% = 320 HH
- Backend (Semi): 8 semanas × 100% = 320 HH
- Frontend (Semi): 8 semanas × 100% = 320 HH
- QA Lead (Semi): 4 semanas × 100% = 160 HH
- QA Jr: 3 semanas × 100% = 120 HH
- DevOps (Semi): 10 semanas × 50% = 200 HH
- PM (Sénior): 10 semanas × 20% = 80 HH

**Total típico: ~1620 HH**

### 2. TARIFAS INTERNAS (COSTO)

Costo por hora (incluye salario + overhead + beneficios):
- Sénior: $40-50 USD/HH
- Semi-Sénior: $25-35 USD/HH
- Junior: $15-20 USD/HH

**NO CONFUNDAS:** Esto es lo que le cuesta a ELITSOFT estar trabajando.

### 3. INFRAESTRUCTURA (COSTO PARA ELITSOFT)

/mes típico:
- Hosting DEV: $100-200
- Hosting STAGING: $200-400
- Hosting PROD: $500-1000 (según escala)
- Licencias tools: $100-500 (Jira, Confluence, APM, etc)
- CDN: $50-200
- Monitoreo: $50-100

Duración: 10-12 semanas típicamente

### 4. COSTO TOTAL PROJECT

```
1620 HH × $30/HH promedio = $48,600 (RH)
+ infra (12 meses) ≈ $3,000
+ contingencia 10% = $5,160
─────────────────────────────────
COSTO TOTAL = ~$56,760
```

### 5. PRECIO VENTA (MARGEN)

**Objetivo típico: 40% margen**

```
Costo:            $56,760
Margen 40%:       $22,704
─────────────────────────
Subtotal venta:   $79,464
IVA 19%:          $15,098
─────────────────────────
TOTAL CLIENTE:    $94,562 USD
```

**Validación:** Margen debe ser 30-50% típicamente.

### 6. ESTRUCTURA DE PAGO

Típicamente 4 cuotas:
- 30% ($28,369) al firmar
- 20% ($18,912) hito diseño
- 30% ($28,369) hito MVP
- 20% ($18,912) go-live

---

## Output Esperado

Documento que muestre:
- ✅ Equipo detallado con HH
- ✅ Costo interno por rol
- ✅ Costos infra
- ✅ Costo total proyecto
- ✅ Precio venta (con margen)
- ✅ Estructura de pago 4 cuotas
- ✅ Análisis rentabilidad
- ✅ Escenarios pesimista/optimista
- ✅ Riesgos financieros

---

**Próximo paso:** pasar a prompt_generador para generar documento formal
