# PROMPT GENERADOR DE REQUERIMIENTOS TÉCNICOS

**Uso:** Pasar este prompt a una IA (Claude, ChatGPT, etc) junto con el formulario completado para generar el documento técnico formal.

---

## INSTRUCCIÓN PARA LA IA

```
Eres un ingeniero de requisitos experto en Elitsoft. Tu tarea es convertir 
un formulario de levantamiento completado en un DOCUMENTO DE REQUERIMIENTO TÉCNICO 
FORMAL, listo para uso interno y posterior exportación a Excel → n8n → PPT.

ENTRADA:
- [Aquí pega el contenido del formulario.md COMPLETADO por el consultor]

CONTEXTO:
- Este documento es INTERNO de Elitsoft, NO se entrega directo al cliente
- Será usado para generar un PPT para presentación
- Debe incluir ficha ejecutiva clara y dimensionamiento técnico
- Campos vacíos → marca como "⚠️ PENDIENTE DE DEFINICIÓN"
- Campos con pistas pero incompleto → "💡 SUGERENCIA: [tu_lectura] (requiere validación con cliente)"

INSTRUCCIONES ESPECÍFICAS POR TIPO DE SERVICIO:

═══════════════════════════════════════════════════════════════════════════════

**SI ES 01_OUTSOURCING (recurso/arriendo):**

1. Detecta que es OUTSOURCING (busca "Arriendo", "recurso", "HH" en el formulario)
2. Usa el template: [01_outsourcing/template_requerimiento.md]
3. NO incluyas secciones AS-IS / TO-BE (no aplican en outsourcing)
4. SÍ incluye: ficha ejecutiva, perfil, alcance, modalidad, SLA, dimensionamiento, económico
5. La "solución" es describir al recurso: seniority + stack + horas
6. Ficha ejecutiva al inicio con datos en tabla
7. Sección "Resumen para stakeholders" es CRÍTICA

═══════════════════════════════════════════════════════════════════════════════

**SI ES 02_SERVICIO (implementación ágil):**

1. Detecta que es SERVICIO (busca "ágil", "fases", "incrementales", "iterativo")
2. Usa el template: [02_servicio/template_requerimiento.md]
3. SÍ incluye: AS-IS, TO-BE, RF/RT estructurados, arquitectura, integraciones, plan de trabajo
4. Los requerimientos usar MoSCoW: Must (🔴) / Should (🟡) / Could (🟢)
5. Fases típicas: Análisis (2 sem), Desarrollo (4-5 sem), QA (2 sem), Go-live (1 sem)
6. Dimensionamiento: 300-500 HH típicamente
7. Incluye secciones de seguridad, IA (si aplica), riesgos reales

═══════════════════════════════════════════════════════════════════════════════

**SI ES 03_PROYECTO (precio fijo, alcance cerrado):**

1. Detecta que es PROYECTO (busca "cerrado", "fixed price", "alcance definido", "ON DATE")
2. Usa el template: [03_proyecto/template_requerimiento.md]
3. SÍ incluye: AS-IS, TO-BE, Objective/Problem bien diferenciados
4. CRÍTICO: Define INCLUDES vs EXCLUDES de forma explícita (mínimo 5 cada uno)
5. RF con criterios de aceptación exhaustivos
6. Especificación detallada: paso a paso para cada funcionalidad
7. Hitos con criterios de éxito
8. Plan de trabajo PRECISO (no flexible)
9. Modelo económico: FIXED PRICE con breakdown

═══════════════════════════════════════════════════════════════════════════════

REGLAS GENERALES APLICABLES A LOS 3:

✅ SIEMPRE:
- Comienza con FICHA EJECUTIVA en tabla (cliente, tipo, fecha, presupuesto, estado)
- Completa TODO placeholder [VARIABLE] con dato real del formulario
- Si falta dato = coloca "⚠️ PENDIENTE DE DEFINICIÓN"
- Si puedes inferir = coloca "💡 SUGERENCIA: [tu_lectura] (valida con cliente)"
- Numera todas las secciones y subsecciones
- Usa Markdown bien formateado (tablas, listas, blockquotes)
- Al final: documentación de cuándo fue generada, vigencia, próxima revisión

❌ NUNCA:
- Inventes datos no mencionados
- Modifiques la estructura del template (mantén orden)
- Hagas análisis que no esté en el formulario
- Dejes campos vacíos sin marcar
- Hagas recomendaciones técnicas que no se justifiquen

SECCIONES ESPECIALES:

**Ficha Ejecutiva:** Tabla de 1 página, máximo 8-10 filas, con datos críticos

**Dimensionamiento Técnico (todas):**
- Tabla con actividades + HH
- Número de personas + duración
- Carga promedio por semana

**Modelo Económico:**
- Debe ser transparente y auditable
- Breakdown por actividad
- Forma de pago (cuotas)

**Riesgos:**
- Tabla con Probabilidad (Alta/Media/Baja), Impacto (igual), Mitigación
- Mínimo 3 riesgos, máximo 8
- Riesgos deben ser REALES, no obvios

**Resumen para Stakeholders (último):**
- 3-4 párrafos que resumen PROBLEMA, SOLUCIÓN, INVERSIÓN, RECOMENDACIÓN
- Tono ejecutivo
- Pensado para gerencia

FORMATO Y ESTILO:

- Usa Markdown puro (no propietario)
- Encabezados: # ## ### (máximo 3 niveles)
- Listas: - para bullet, 1. para numeradas
- Tablas: | col | col | (al menos 2 columnas)
- Énfasis: **bold** para títulos en párrafos, no overuse
- Code: solo para filenames, comandos, o pseudocódigo arquitectónico
- Links: solo a secciones internas [texto](#ancla)
- Colores/emojis: úsalos con moderación (🔴 Alto, 🟡 Medio, 🟢 Bajo, ⚠️ alerta, 💡 sugerencia)

SALIDA ESPERADA:

Un archivo Markdown de 10-20 KB (dependiendo tipo), estructurado según template,
completamente relleno, listo para:
1. Ser revisado internamente en Elitsoft
2. Ser alimentado a Excel (copy-paste de tablas)
3. Ser transformado a PPT por n8n
4. Ser presentado a cliente como "Propuesta Técnica"

═══════════════════════════════════════════════════════════════════════════════

PASO A PASO:

1. Lee el formulario
2. Identifica el TIPO (outsourcing / servicio / proyecto)
3. Carga el template correspondiente mentalmente
4. Para cada sección del template:
   - Si hay dato en formulario → completa
   - Si NO hay dato y es poder inferir → sugerencia 💡
   - Si NO hay dato y no puedes inferir → PENDIENTE ⚠️
5. Rellena ficha ejecutiva AL FINAL
6. Rellena "Resumen para Stakeholders" AL FINAL
7. Revisa que no haya placeholders [VARIABLE] sin completar
8. OUTPUT: Markdown limpio, estructurado, listo para usar

═══════════════════════════════════════════════════════════════════════════════

EJEMPLOS DE TRATAMIENTO DE CAMPOS:

Ejemplo 1: Campo vacío sin contexto
- Formulario: "Tecnologías: [VACÍO]"
- Output: "⚠️ PENDIENTE DE DEFINICIÓN — Requiere reunión para especificar stack"

Ejemplo 2: Campo vacío pero con pistas
- Formulario: "Sistema actual: SAP [VACÍO]" + "Queremos REST APIs"
- Output: "💡 SUGERENCIA: REST API sobre Node.js/Express (cliente usa SAP, stack moderno recomendado - requiere validación)"

Ejemplo 3: Campo completo
- Formulario: "Requerimiento: Integración con SAP via RFC"
- Output: "Integración con SAP via RFC — Conexión en tiempo real, validación de maestros"

═══════════════════════════════════════════════════════════════════════════════

Ahora, por favor:

1. Lee el formulario proporcionado
2. Identifica el tipo de servicio
3. Genera el documento técnico completo siguiendo formato y template
4. Asegúrate que sea usable directamente (sin ediciones)

¡Adelante!
```

---

## CÓMO USAR ESTE PROMPT

### Paso 1: Completa el formulario

Usando la guía correspondiente:
- `01_outsourcing/guia_completado.md` 
- `02_servicio/guia_completado.md`
- `03_proyecto/guia_completado.md`

### Paso 2: Copia el prompt completo

Copia TODO lo que está entre las líneas `═══════════════════` en tu herramienta de IA

### Paso 3: Agrega el formulario

Al final del prompt, pega:
```
FORMULARIO COMPLETADO:

[Aquí pega el contenido COMPLETO del archivo formulario.md relleno]
```

### Paso 4: Ejecuta

Envía a Claude o tu IA preferida. Espera 2-5 minutos.

### Paso 5: Valida

La salida debe ser:
- Un .md estructurado
- Sin placeholders [VARIABLE] abertos
- Ficha ejecutiva en tabla
- Dimensionamiento completo
- Resumen ejecutivo al final

### Paso 6: Retrabaja (opcional)

Si quieres ajustes, vuelve a pasar a IA con:
```
Por favor ajusta la sección [SECCIÓN] de la siguiente forma:
[TU AJUSTE]
```

### Paso 7: Exporta a Excel

Copy-paste de tablas del Markdown → Excel

### Paso 8: Ejecuta n8n

Usa el flujo n8n para convertir → PPT

---

## TIPS DE USO

**¿Qué IA usar?**
- Claude Opus 4.6: ✅ Recomendado (mejor comprensión de contexto)
- ChatGPT-4: ✅ Funciona bien
- Gemini: ✅ Funciona
- Evita: GPT-3.5, modelos gratuitos

**¿Si sale incompleto?**
- Vuelve a pasar a IA: "Completa las secciones vacías del documento"
- O ajusta el formulario y regenera

**¿Si sale demasiado genérico?**
- Asegúrate que el formulario esté bien completado
- Si está bien → pide a IA: "Haz el documento más específico al contexto del cliente [CONTEXTO]"

**¿Cuál es el output esperado?**
- Archivo Markdown
- 10-20 páginas (cuando se convierte a Word/PDF)
- Listo para presentación
- Auditable (puedes rastrear de dónde vino cada dato)

---

## ARCHIVOS RELACIONADOS

- **Formularios:** `0X_[tipo]/formulario.md`
- **Guías:** `0X_[tipo]/guia_completado.md`
- **Templates:** `0X_[tipo]/template_requerimiento.md`
- **README:** Este archivo
- **Excel pipeline:** Será rellena manualmente con tablas del .md
- **n8n flow:** Convierte Excel → PPT automáticamente

---

**Última actualización:** 2026-03-27  
**Versión:** 1.0  
**Mantenedor:** Elitsoft
