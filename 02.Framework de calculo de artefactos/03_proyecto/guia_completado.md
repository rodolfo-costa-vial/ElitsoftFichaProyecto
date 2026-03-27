# GUÍA — CÁLCULO DE ARTEFACTOS TÉCNICOS (PROYECTO CERRADO)

**Uso interno Elitsoft**

---

## ¿Qué Es?

Documento exhaustivo que lista TODOS los artefactos técnicos a desarrollar/validar en el proyecto, con especificaciones y criterios de aceptación por cada uno.

---

## Cómo Completar

### 1. LISTA COMPLETA DE ARTEFACTOS

Enumera TODOS (no dejes fuera nada):

**Backend:**
- API 1: especificación, endpoints
- API 2: especificación, endpoints
- Servicio 1: descripción, alcance
- etc.

**Frontend:**
- Pantalla 1: descripción, workflows
- Pantalla 2: descripción, workflows
- Componentes UI: tipos, cantidad
- etc.

**Database:**
- Tabla 1: campos, índices, relaciones
- Tabla 2: campos, índices, relaciones
- etc.

**Infra/DevOps:**
- Servidores: specs, cantidad
- Networking: configuración
- Storage: capacidad, tiering
- CI/CD: herramientas, flujo
- Monitoreo: herramientas, alertas

**Testing:**
- Unit: cobertura target (80%+)
- Integration: escenarios
- E2E: escenarios
- Performance: specs
- Security: specs

**Documentación:**
- API docs: Swagger/OpenAPI
- Architecture: diagrama + texto
- Deployment guide: paso a paso
- User manual: video + docs
- Runbooks: operación

### 2. DoD POR ARTEFACTO

Cada artefacto tiene checklist:
- ☑ Código en repo
- ☑ Compilable sin warnings
- ☑ Tests pasan
- ☑ Security OK
- ☑ Performance OK
- ☑ Documentado
- ☑ Code review aprobado

### 3. HITOS

Define puntos de validación:
- Hito 1 (Semana 2): Backend APIs + DB schema
- Hito 2 (Semana 4): Frontend + APIs integradas
- Hito 3 (Semana 6): Testing + docs
- Hito 4 (Semana 8): UAT ready

### 4. MATRIZ MASTER

Una tabla con TODOS los artefactos:
- Nombre
- Tipo (Componente, API, Screen, etc)
- Tecnología
- Especificación
- DoD Check (checkbox)
- Status

---

## Output Esperado

Documento que muestre:
- ✅ Inventario completo de artefactos
- ✅ Qué especificación cumple cada uno
- ✅ Qué hitos tienen validación
- ✅ Qué DoD aplica
- ✅ Timeline de completion
- ✅ Sign-off de tech leads

---

**Próximo paso:** pasar a prompt_generador para generar documento formal
