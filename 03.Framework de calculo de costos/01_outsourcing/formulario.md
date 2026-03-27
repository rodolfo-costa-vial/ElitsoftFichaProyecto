# FORMULARIO — CÁLCULO DE COSTOS
## OUTSOURCING (Recurso)

**Cliente:**  
**Recurso:**  
**Fecha:**  
**Período:**  

---

## 1. DIMENSIONAMIENTO DE HORAS

### 1.1 Estimación Mensual
- Horas/semana: [N]
- Semanas/mes: [N] (tipicamente 4.33)
- Total HH/mes: [CÁLCULO: HH/sem × 4.33]

### 1.2 Duración del Recurso
- Mes inicio: [MES]
- Mes fin: [MES]
- Total meses: [N]
- **Total HH proyecto:** [MESES × HH/mes]

### 1.3 Desglose por Actividad (opcional)
- Análisis/diseño: [%]
- Desarrollo: [%]
- Testing: [%]
- Soporte: [%]

---

## 2. ESTRUCTURA DE COSTOS

### 2.1 Tarifa
- Seniority: [JUNIOR/SEMI-SENIOR/SENIOR/LEAD]
- Tarifa base (USD/HH): [TARIFA]
- Contingencia: [%]
- **Tarifa final (USD/HH):** [(TARIFA × (1 + contingencia%))]

### 2.2 Cálculo Mensual
```
Costo mensual = HH/mes × Tarifa/HH
Costo mensual = [HH] × [USD/HH] = [TOTAL] USD/mes
```

### 2.3 Cálculo Total
```
Costo total = Total HH proyecto × Tarifa/HH
Costo total = [HH] × [USD/HH] = [TOTAL] USD
```

---

## 3. ANÁLISIS DE RENTABILIDAD

### 3.1 Márgenes Internos
- Costo Elitsoft (salario + overhead): [COSTO_INTERNO_HH]
- Tarifa venta: [TARIFA_VENTA_HH]
- Margen bruto: [(VENTA - COSTO) / VENTA × 100]%

### 3.2 Impacto en Proyecto
- Ingresos: [TOTAL_VENTA]
- Costo directo: [TOTAL_COSTO]
- **Margen proyecto:** [MARGEN] USD / [%]

---

## 4. VARIABLES DE RIESGO

- ¿Recurso puede trabajar menos horas? [SÍ/NO] → Impacto: [IMPACTO]
- ¿Recurso puede enfermarse? [SÍ/NO] → Impacto: [IMPACTO]
- ¿Cliente extiende plazo? [SÍ/NO] → Impacto: [IMPACTO]

---

## 5. OBSERVACIONES

[NOTAS_COMERCIALES]
