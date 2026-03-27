# GUÍA — CÁLCULO DE ARTEFACTOS TÉCNICOS (OUTSOURCING)

**Uso interno Elitsoft**

---

## ¿Qué Es?

Documento que lista y valida TODOS los componentes técnicos que el recurso outsourcing debe entregar/mantener.

---

## Cómo Completar

### 1. COMPONENTES TÉCNICOS

**Pregunta:** "¿Qué sistemas, servidores, aplicaciones va a tocar este recurso?"

Respuesta debe incluir:
- Infraestructura (servidores, redes, storage)
- Aplicaciones (qué code bases, frameworks)
- Bases de datos (cuáles)
- Integraciones (con qué sistemas externos)

### 2. CUMPLIMIENTO DE ESPECIFICACIONES

**Pregunta:** "¿Cómo validates que todo funciona bien?"

Definir:
- Performance: "Respuesta <2 seg en 95th percentile"
- Seguridad: "Encriptación TLS 1.2+"
- Escalabilidad: "Soportar 10x crecimiento"
- Disponibilidad: "99.5% uptime"

### 3. CHECKLIST

Crear tabla con cada componente y si está "validated" (checkbox)

### 4. RIESGOS

Listar riesgos técnicos específicos (legacy, deuda técnica, etc)

---

## Output Esperado

Documento ejecutivo que muestre:
- ✅ Qué artefactos entrega/mantiene el recurso
- ✅ Qué cumple especificación
- ✅ Qué documentación existe
- ✅ Qué riesgos hay

---

**Próximo paso:** pasar a prompt_generador para generar documento formal
