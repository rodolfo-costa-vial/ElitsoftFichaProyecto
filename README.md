# FRAMEWORK DE LEVANTAMIENTO DE REQUERIMIENTOS — ELITSOFT

**Última actualización:** 27 de marzo de 2026  
**Versión:** 2.0  
**Estado:** ✅ Operativo

---

## 📋 Descripción General

Framework estructurado para convertir información de clientes en documentos de requerimientos técnicos formales. Diseñado para uso interno de Elitsoft, alimenta pipeline: Formulario → Documento → Excel → n8n → PPT Ejecutivo.

---

## 🏢 Tres Productos = Tres Flujos

| Producto | Carpeta | Formulario | Template | Guía |
|----------|---------|-----------|----------|------|
| **Outsourcing** | `01_outsourcing/` | formulario.md | template_requerimiento.md | guia_completado.md |
| **Servicio Ágil** | `02_servicio/` | formulario.md | template_requerimiento.md | guia_completado.md |
| **Proyecto Cerrado** | `03_proyecto/` | formulario.md | template_requerimiento.md | guia_completado.md |

---

## 🔄 Flujo de Trabajo

### Paso 1: Elige Producto

Pregúntate: ¿Qué está vendiendo Elitsoft aquí?

- **01_OUTSOURCING:** Cliente necesita un **recurso** (persona)  
  → Modelo: Horas Hombre (HH)  
  → No hay AS-IS/TO-BE

- **02_SERVICIO:** Cliente tiene idea general, **alcance flexible**  
  → Modelo: Proyecto con fases  
  → Incluye AS-IS/TO-BE

- **03_PROYECTO:** Cliente tiene requerimiento **100% claro**  
  → Modelo: Precio Fijo  
  → Alcance cerrado, incluye AS-IS/TO-BE

---

### Paso 2: Lee la Guía

Abre la guía correspondiente (`guia_completado.md`):
- Qué preguntas hacer
- Qué documento completar
- Qué riesgos evitar
- Checklist antes de terminar

---

### Paso 3: Completa el Formulario

Rellena `formulario.md` EN REUNIÓN CON EL CLIENTE:
- No asumir información
- Validar supuestos
- Documentar riesgos y exclusiones

---

### Paso 4: Genera Documento Técnico

Usa `prompt_generador.md`:
- Copia el prompt completo
- Pega el formulario relleno
- Envía a Claude/ChatGPT
- Recibe documento formal automáticamente

---

### Paso 5: Retrabaja (Elitsoft Interno)

Valida, ajusta, enriquece:
- ¿Dimensionamiento tiene sentido?
- ¿Riesgos son reales?
- ¿Presupuesto es competitivo?

---

### Paso 6: Export → Excel

Copy-paste de tablas del Markdown a Excel

---

### Paso 7: n8n Flow

Excel → PowerPoint automático

---

### Paso 8: Presenta a Cliente

PPT con propuesta técnica y económica

---

## 📁 Estructura de Carpetas

```
ElitsoftFichaProyecto/
│
├── 01_outsourcing/
│   ├── formulario.md                ← Completa en reunión
│   ├── template_requerimiento.md    ← Referencia (auto-usado por IA)
│   └── guia_completado.md           ← Lee ANTES de empezar
│
├── 02_servicio/
│   ├── formulario.md
│   ├── template_requerimiento.md
│   └── guia_completado.md
│
├── 03_proyecto/
│   ├── formulario.md
│   ├── template_requerimiento.md
│   └── guia_completado.md
│
├── prompt_generador.md              ← El prompt maestro
├── README.md                        ← Este archivo
├── .gitignore                       ← Configuración git
└── [Documentación de referencia]
```

---

## ⚡ Uso Rápido

### Para Consultor — Primer Contacto

1. **¿Qué vende?**
   - Recurso → `01_outsourcing`
   - Implementación → `02_servicio`
   - Proyecto fijo → `03_proyecto`

2. **Lee guía:** `0X_[tipo]/guia_completado.md` (15 min)

3. **Completa formulario:** `0X_[tipo]/formulario.md` en reunion (60-90 min)

4. **Entrega a Arquitecto:** "Formulario completado, ¿revisas?"

### Para Arquitecto — Generación Documento

1. Recibe formulario completado

2. Copia contenido de `prompt_generador.md`

3. Pega el formulario al final del prompt

4. Envía a Claude

5. Revisa salida (10 min)

6. Si necesita ajustes: re-inicia paso 3

7. Exporta versión final a Excel

### Para Comercial — Presentación

1. Recibe Excel con datos extraídos

2. Ejecuta n8n flow

3. Descarga PPT

4. Presenta a cliente

---

## 💡 Tips Importantes

### Cómo Distinguir Productos

| Pregunta Cliente | Respuesta → Producto |
|-----------------|----------------------|
| "Necesito un especialista part-time" | → 01_outsourcing |
| "Tenemos un proyecto que necesitamos entregar, no estamos seguros cómo" | → 02_servicio |
| "Sabemos exactamente qué necesitamos, ¿cuánto cuesta?" | → 03_proyecto |

### Campos Vacíos en Documento Generado

**Si sale `⚠️ PENDIENTE DE DEFINICIÓN`:**
- Falta información en el formulario
- Vuelve con cliente para completar
- O re-genera documento después

**Si sale `💡 SUGERENCIA`:**
- IA está completando gaps inteligentemente
- Valida con cliente/arquitecto
- Es aceptable pero no definitivo

### Cómo Validar Dimensionamiento

- Outsourcing: HH = (horas/semana × semanas × 4.33) / 8
- Servicio: Típico 300-500 HH total
- Proyecto: Típico 250-400 HH total

Si salen 1000+ HH → sospechar. ¿Es realmente un proyecto o es diagnostico?

---

## 🎯 Casos de Uso

### Caso 1: Cliente necesita dev part-time por 6 meses

```
→ Producto: 01_OUTSOURCING
→ Usar: 01_outsourcing/formulario.md
→ Leer: 01_outsourcing/guia_completado.md
→ Perfil: Senior/Semi-senior
→ Presupuesto: HH × Tarifa × 6 meses
→ Documento: Sin AS-IS/TO-BE
```

### Caso 2: Cliente tiene idea, quiere implementar por fases

```
→ Producto: 02_SERVICIO
→ Usar: 02_servicio/formulario.md
→ Leer: 02_servicio/guia_completado.md
→ Requerimientos: MoSCoW (Must/Should/Could)
→ Plazo: 9-12 semanas típico
→ Documento: Con AS-IS/TO-BE, especificación
```

### Caso 3: Cliente tiene requirements board, necesita presupuesto fijo

```
→ Producto: 03_PROYECTO
→ Usar: 03_proyecto/formulario.md
→ Leer: 03_proyecto/guia_completado.md
→ Alcance: Cierro en formulario (INCLUDES/EXCLUDES)
→ Presupuesto: Fixed price
→ Documento: Exhaustivo, con hitos y criterios aceptación
```

---

## ✅ Checklist Antes de Generar Documento

### Formulario Completado

- ☐ Información cliente: sí
- ☐ Contexto/problema: específico
- ☐ Sistema actual (AS-IS): documentado
- ☐ Objetivo (TO-BE): claro
- ☐ Requerimientos: estructurados
- ☐ Riesgos: al menos 3, reales
- ☐ Supuestos: documentados
- ☐ Exclusiones: documentadas

### Antes de Pasar a IA

- ☐ Formulario está COMPLETAMENTE relleno (o marcado PENDIENTE)
- ☐ No tiene más de 20 campos vacíos
- ☐ Cliente validó la info

### Después de Generar

- ☐ Documento tiene estructura completa
- ☐ No hay placeholders [VARIABLE] abiertos
- ☐ Ficha ejecutiva legible
- ☐ Dimensionamiento auditable
- ☐ Modelo económico claro

---

## 🔐 Confidencialidad

Este framework es **INTERNO ELITSOFT** solamente.

- No compartas formularios con cliente (sin aprobación)
- No compartas documento draft hasta final
- Document final (PPT) es lo que se presenta

---

## 🚀 Próximos Pasos

1. **Completa el primer formulario** (cualquiera de los 3)
2. **Usa el prompt generador** para generar documento
3. **Valida el flujo** end-to-end
4. **Ajusta templates** si es necesario
5. **Integra con Excel** → n8n → PPT

---

## 📞 Soporte

**¿Dudas sobre qué producto elegir?**  
Lee `0X_[tipo]/guia_completado.md` → sección "¿Cuándo usar"

**¿Formulario no tiene campo que necesito?**  
Agrega a template, re-genera

**¿Documento no tiene suficiente detalle?**  
Completa formulario + re-genera

**¿Prompt no funciona bien?**  
Valida: ¿formulario está muy incompleto? Si sí → completa primero

---

**Última actualización:** 27-03-2026  
**Versión:** 2.0  
**Responsable:** Elitsoft Ingeniería
