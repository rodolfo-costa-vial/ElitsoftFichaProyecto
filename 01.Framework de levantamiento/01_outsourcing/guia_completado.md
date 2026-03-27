# GUÍA PARA COMPLETAR FORMULARIO — OUTSOURCING

**Uso interno Elitsoft**

---

## ¿Cuándo usar este modelo?

✅ **Usar OUTSOURCING cuando:**
- El cliente necesita un **recurso** (persona), no un entregable
- El scope NO está 100% definido
- Se requiere apoyo continuo o "estar disponible"
- El cliente controla la agenda (disponibilidad horaria)
- Modelo de negocio: Horas Hombre (HH)

❌ **NO usar cuando:**
- Hay un proyecto definido con entregables claros → usar SERVICIO o PROYECTO
- El cliente no sabe qué necesita exactamente → primera hacer diagnóstico

---

## Consejos por sección

### FICHA EJECUTIVA
- Llena al final, resumen de lo que recolectaste
- Cliente + Consultor + Area + Estado siempre

### 1. CONTEXTO GENERAL

**¿Qué preguntar?**
- "¿En qué industria trabajan?" (Finanzas, Retail, Manufactura, etc.)
- "¿Cuántos empleados tiene la compañía?" (Startup, PyME, Corporativa)
- "¿Cuál es el área que está solicitando?" (IT, Operaciones, Finanzas, etc.)

**Errores comunes:**
- Poner "IT" como área si no es específico → preguntar qué equipo dentro de IT
- No validar industria → afecta el contexto técnico

---

### 2. NECESIDAD DEL CLIENTE

**¿Qué preguntar?**
- "¿Cuál es el principal desafío HOY?" (escúchalo sin interrumpir)
- "¿Qué sistemas usan actualmente?" (SAP, Oracle, legacy, etc.)
- "¿Quién es la contraparte interna?" (el que trabajará con el recurso)

**Rojo de alerta:**
- Si dicen "no sabemos exactamente qué necesitamos" → sugerir diagnóstico PRIMERO
- Si hay muchas integraciones → preguntar documentación de APIs

---

### 3. PERFIL REQUERIDO

**El perfil es CRÍTICO en outsourcing.**

**¿Qué preguntar?**
- "¿Necesitan alguien sénior o semi-sénior?" 
- "¿Qué lenguajes/stacks específicos?" (no preguntes "qué tech", sé preciso)
- "¿Necesita liderazgo de equipo o solo ejecución?"

**Seniority típico:**
- Junior (1-3 años): soporte básico, testing
- Semi-Sénior (3-8 años): desarrollo sin arquitectura
- Sénior (8+ años): diseño, arquitectura, decisiones
- Lead (10+ años): liderazgo + ejecución

---

### 4. ALCANCE DEL SERVICIO

**¿Qué preguntar?**
- "¿Qué hará el recurso DÍA 1?" (esto es clave)
- "¿Cada cuánto necesitan tareas/assigment nuevo?"
- "¿Habrá documentación que generar?"

**Responsabilidades:**
- Cliente SIEMPRE: acceso a sistemas + validaciones + decisiones
- Elitsoft SIEMPRE: realizar las tareas + reportar avance

---

### 5. MODALIDAD DE TRABAJO

**Preguntas obligatorias:**
- "¿Dónde trabajará? ¿Remoto o presencial?"
- "¿Mismo horario del cliente o flexible?"
- "¿Qué herramientas usan?" (Slack, Teams, Jira, Azure DevOps, etc.)

**Red flag:**
- Si dicen "presencial" pero están fuera del país → costo adicional de viaje

---

### 6. CAPACITACIÓN

**¿Se requiere transferencia de conocimiento?**
- Casi siempre SÍ en outsourcing
- Preguntar: "¿Quién capacitará al recurso? ¿Cuánto tiempo?"
- Si NO hay nadie → sugerir documentación mínima

---

### 7. ONBOARDING

**Accesos necesarios:**
- VPN, repositorios, BD, servidores, sistemas externos
- Pregunta: "¿Cuánto tarda en dar accesos?" (puede retrasar inicio)

**Contraparte:**
- Nombre + email + rol específico
- Esta persona será la que briefe diariamente al recurso

---

### 8. SLA Y EXPECTATIVAS

**Preguntar:**
- "¿Si el recurso se enferma, cuánto tiempo pueden esperar a un reemplazo?"
- "¿Nivel de disponibilidad esperado?" (8x5, 24x7, etc.)

---

### 9. PLAZO

**Preguntar:**
- "¿Cuánto tiempo necesitarán el recurso?" (3 meses, 1 año, indefinido)
- "¿Es renovable o contrato terminado?"

---

### 10. DIMENSIONAMIENTO TÉCNICO

**Cálculo de horas:**
- Onboarding: normalmente 1-2 semanas
- Mes 1: puede ser full-time o part-time dependiendo de lo que descubran
- Proyectar solo 3 meses con visibilidad, el resto "renovable"

**Equipo:**
- Normalmente 1 recurso, a veces 2 si es proyecto grande

---

### 11. MODELO ECONÓMICO

**Cálculo:**
- Buscar tarifa interna para el seniority
- Horas = horas/semana × semanas × 4.33 (promedio de semanas/mes)
- NO sobre-facturar supuestos de horas

**Tip:** Si cliente "no define bien", poner menos horas que más. Es mejor agregar que tener sorpresas.

---

### 12. RIESGOS

**Riesgos típicos de outsourcing:**
- Alcance unclear → cliente pide "más"
- Accesos lentos → retrasos en inicio
- Contraparte indisponible → no hay direction
- Stack legacy → difícil encontrar recurso

---

### 13. SUPUESTOS

**Típicos:**
- "Cliente proporciona accesos en semana 1"
- "Documentación técnica está disponible"
- "Contraparte dedicada dedica 4 horas/semana"

---

### 14. EXCLUSIONES

**Típicas:**
- "No incluye arquitectura empresarial"
- "No incluye gestión de proyecto"
- "No incluye capacitación a otros usuarios"

---

## Checklist antes de entregar

- ☐ ¿Tiene al menos 1 contacto en el cliente?
- ☐ ¿El perfil está específico? (no solo "developer")
- ☐ ¿Las horas tienen lógica matemática?
- ☐ ¿Los riesgos son reales o son obvios?
- ☐ ¿El cliente validó los supuestos?
- ☐ ¿Hay al menos 2 exclusiones?

---

## Próximo paso

Una vez completado esté formulario → pasar a **prompt_generador.md** para generar el documento técnico formal
