# GUÍA — CÁLCULO DE ARTEFACTOS TÉCNICOS (SERVICIO ÁGIL)

**Uso interno Elitsoft**

---

## ¿Qué Es?

Documento que describe TODOS los artefactos a entregarse por fase, con especificaciones y criterio de aceptación.

---

## Cómo Completar

### 1. ARTEFACTOS POR FASE

**Pregunta:** "¿Qué va a entregar cada fase?"

- Fase 1: APIs base, DB, UI básica → MVP mínimo
- Fase 2: Integraciones, features, testing exhaustivo
- Fase N: Go-live, documentación, capacitación

**Para cada artefacto especificar:**
- Qué es (componente, API, pantalla, doc)
- Por qué (necesidad de negocio)
- Cómo validar (DoD: Definition of Done)

### 2. DoD (DEFINITION OF DONE)

Cada artefacto tiene checklist:
- ☑ Código compilable
- ☑ Tests pasan (80%+ coverage)
- ☑ Security scan OK
- ☑ Performance OK
- ☑ Documentado

### 3. ESPECIFICACIONES TÉCNICAS

Por cada tipo de artefacto (Backend/Frontend/DB):
- Stack usado
- Número de componentes
- Targets de performance
- Documentación completada

### 4. QUALITY GATES

Tabla con métricas clave que todo artefacto debe cumplir:
- Test coverage >80%
- Performance <2seg
- 0 vulnerabilidades críticas
- Code review 100% pasado

---

## Output Esperado

Documento que muestre:
- ✅ Qué artefactos por fase
- ✅ Qué cumple DoD
- ✅ Qué métricas de quality
- ✅ Qué dependencias/blockers
- ✅ Timeline de completion

---

**Próximo paso:** pasar a prompt_generador para generar documento formal
