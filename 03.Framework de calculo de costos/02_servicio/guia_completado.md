# GUÍA — CÁLCULO DE COSTOS (SERVICIO ÁGIL)

**Uso interno Elitsoft**

---

## ¿Qué Es?

Documento que calcula presupuesto total, desglose de costos y análisis de rentabilidad para un proyecto ágil.

---

## Cómo Completar

### 1. EQUIPO Y HH

**Pregunta:** "¿Quiénes van a trabajar y cuántas horas?"

Estructura típica:
- Tech Lead (Sénior): 30% dedicación × 10 semanas = 120 HH
- Backend Dev (Semi): 100% × 8 semanas = 320 HH
- Frontend Dev (Semi): 100% × 8 semanas = 320 HH
- QA (Junior): 100% × 3 semanas = 120 HH
- PM (Sénior): 20% × 10 semanas = 80 HH

**Total: ~950 HH**

### 2. TARIFA POR PERFIL

Tarifas internas (ajusta):
- Sénior: $60 USD/HH
- Semi-Sénior: $45 USD/HH
- Junior: $30 USD/HH

### 3. INFRAESTRUCTURA

Costos típicos/mes:
- Hosting: $500-1000
- Licencias: $100-500 (one-time o monthly)
- CDN: $50-200
- Mail/SMS: $100-300

**Duración:** 10-12 semanas típicamente

### 4. CONTINGENCIA

Suma 10-15% por:
- Alcance creep
- Delays integraciones
- Bugs inesperados

### 5. PAGO

Estructura de 4 cuotas (30-20-30-20):
- Anticipo: 30% al firmar
- Hito 1 (Diseño): 20% 
- Hito 2 (MVP): 30%
- Go-live: 20%

---

## Output Esperado

Documento que muestre:
- ✅ Equipo y HH por rol
- ✅ Costos desglosados por fase
- ✅ Presupuesto total con IVA
- ✅ Estructura de pago
- ✅ Margen rentabilidad
- ✅ Escenarios (optimista/pesimista)

---

**Próximo paso:** pasar a prompt_generador para generar documento formal
