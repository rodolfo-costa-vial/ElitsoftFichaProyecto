# REQUERIMIENTO TÉCNICO — SERVICIO ÁGIL
**Generado automáticamente desde formulario de levantamiento**

---

## 📊 FICHA EJECUTIVA

| Parámetro | Valor |
|-----------|-------|
| **Cliente** | [CLIENTE] |
| **Tipo Servicio** | Implementación Ágil - [N] Fases |
| **Fecha Levantamiento** | [FECHA] |
| **Contacto Elitsoft** | [CONSULTOR] |
| **Problema Clave** | [PROBLEMA_SINTETIZADO] |
| **Duración Estimada** | [DURACIÓN] |
| **Inversión Estimada** | [PRESUPUESTO] USD |
| **Estado** | 🟡 Pendiente validación |

---

## 1. CONTEXTO GENERAL

### 1.1 Situación del Cliente
- **Industria:** [INDUSTRIA]
- **Tamaño:** [TAMAÑO]
- **Área responsable:** [ÁREA]

### 1.2 Objetivo del Servicio
[OBJETIVO]

### 1.3 Problema de Negocio
- **Proceso actual:** [PROCESO_HOY]
- **Desafío:** [DESAFÍO]
- **Impacto negativo:** [IMPACTO]

---

## 2. SITUACIÓN ACTUAL (AS-IS)

### 2.1 Procesos Actuales
[DESCRIPCIÓN_AS_IS]

### 2.2 Sistemas y Herramientas
| Sistema | Versión | Rol |
|---------|---------|-----|
| [SYS1] | [VER] | [ROL] |
| [SYS2] | [VER] | [ROL] |
| [SYS3] | [VER] | [ROL] |

### 2.3 Limitaciones Actuales
**Técnicas:**
- [LIM1]
- [LIM2]

**Operacionales:**
- [LIM3]
- [LIM4]

### 2.4 Volúmenes y Escala
- **Transacciones/día:** [VOL1]
- **Usuarios activos:** [VOL2]
- **Datos almacenados:** [VOL3]

---

## 3. VISIÓN OBJETIVO (TO-BE)

### 3.1 Flujo Esperado
[DESCRIPCIÓN_TO_BE]

### 3.2 Nivel de Automatización
- [AUTO1]
- [AUTO2]
- [AUTO3]

### 3.3 Beneficios Esperados
| Beneficio | Métrica | Valor Esperado |
|-----------|---------|----------------|
| [BEN1] | [MÉTRICA1] | [VALOR] |
| [BEN2] | [MÉTRICA2] | [VALOR] |
| [BEN3] | [MÉTRICA3] | [VALOR] |

---

## 4. REQUERIMIENTOS

### 4.1 Requerimientos Funcionales (RF)

**RF-001:** [FUNCIONALIDAD]
- Descripción: [DESC]
- Prioridad: 🔴 Must / 🟡 Should / 🟢 Could
- Criterios de aceptación:
  - [ ] [CRITERIO1]
  - [ ] [CRITERIO2]

**RF-002:** [FUNCIONALIDAD]
- [...]

### 4.2 Requerimientos Técnicos (RT)

**RT-001:** [REQUERIMIENTO]
- Especificación: [SPEC]
- Restricciones: [REST]

**RT-002:** [REQUERIMIENTO]
- [...]

### 4.3 Requerimientos de Integración

**Sistemas a integrar:**
| Sistema | Tipo | Volumen | Criticidad |
|---------|------|--------|-----------|
| [SYS1] | [TIPO] | [VOL] | 🔴 Alta |
| [SYS2] | [TIPO] | [VOL] | 🟡 Media |

---

## 5. ARQUITECTURA PROPUESTA

### 5.1 Componentes

```
┌──────────────────────────────────┐
│  [Frontend Interface]            │
│  [TECNOLOGÍA]                    │
└──────────────┬───────────────────┘
               │
┌──────────────▼───────────────────┐
│  [API/Servicios]                 │
│  [ARQUITECTURA]                  │
└──────────────┬───────────────────┘
               │
┌──────────────▼───────────────────┐
│  [Base de Datos]                 │
│  [TIPO: PostgreSQL/SQL Server]   │
└──────────────────────────────────┘
```

### 5.2 Stack Tecnológico

| Capa | Tecnología | Justificación |
|------|-----------|---------------|
| Frontend | [TECH] | [RAZÓN] |
| Backend | [TECH] | [RAZÓN] |
| BD | [TECH] | [RAZÓN] |
| Infraestructura | [TECH] | [RAZÓN] |

### 5.3 Integraciones

**[SISTEMA_1]**
- Protocolo: [PROTOCOLO]
- Frecuencia: [FREQ]
- Volumen: [VOL]

**[SISTEMA_2]**
- [...]

### 5.4 Restricciones y Criterios

- **Performance:** [SPEC]
- **Disponibilidad:** [SPEC]
- **Seguridad:** [SPEC]
- **Escalabilidad:** [SPEC]

---

## 6. SEGURIDAD

### 6.1 Autenticación y Autorización
- **Mecanismo:** [AUTH]
- **Proveedores:** [PROV]
- **Roles/Permisos:** [ROLES]

### 6.2 Manejo de Datos
- **Encriptación en tránsito:** [SÍ/NO] - [ESP]
- **Encriptación en reposo:** [SÍ/NO] - [ESP]
- **Clasificación de datos:** [LEVEL]

### 6.3 Auditoría
- **Logs de acceso:** [SÍ/NO]
- **Trazabilidad de cambios:** [SÍ/NO]
- **Retención:** [POLICY]

---

## 7. IA (SI APLICA)

### 7.1 Casos de Uso IA
**[CASO_1]:** [DESCRIPCIÓN]
- Modelo: [MODELO]
- Datos de entrada: [DATOS]
- Datos de salida: [OUTPUT]

### 7.2 Estrategia de Datos
- **Volumen estimado:** [VOL]
- **Calidad esperada:** [%]
- **Entrenamiento:** [FREQ]

---

## 8. PLAN DE TRABAJO

### 8.1 Fases

**FASE 1: ANÁLISIS Y DISEÑO** (Semanas 1-2)
- Refinamiento de requerimientos
- Diseño de arquitectura
- Prototipado de interfaces
- Entregables: Documento de diseño + prototipo

**FASE 2: DESARROLLO (SPRINT 1-2)** (Semanas 3-6)
- Implementación backend
- Implementación frontend
- Integración inicial
- Entregables: MVP + ambiente de testing

**FASE 3: QA Y AJUSTES** (Semanas 7-8)
- Testing funcional
- Testing de integraciones
- Bugs y ajustes
- Entregables: Reporte QA + ambiente pre-producción

**FASE 4: DESPLIEGUE Y CAPACITACIÓN** (Semana 9)
- Deploy a producción
- Capacitación usuarios
- Docs finales
- Entregables: Sistema en vivo + manuales

### 8.2 Priorización (MoSCoW)

**🔴 MUST (Obligatorio):**
- [REQ1]
- [REQ2]

**🟡 SHOULD (Debería):**
- [REQ3]
- [REQ4]

**🟢 COULD (Podría):**
- [REQ5]
- [REQ6]

### 8.3 Dependencias y Supuestos
- Cliente proporciona accesos en día 1
- Documentación técnica del legacy disponible
- Contraparte dedicada 8 horas/semana
- Cambios de requerimiento máximo 2 durante proyecto

---

## 9. EQUIPO

### 9.1 Estructura Elitsoft
| Rol | Seniority | Dedicación | Duración |
|-----|-----------|-----------|----------|
| Tech Lead | Sénior | 50% | 9 semanas |
| Backend Dev | Semi-Sénior | 100% | 8 semanas |
| Frontend Dev | Semi-Sénior | 100% | 8 semanas |
| QA | Junior | 100% | 3 semanas |

### 9.2 Gobierno del Proyecto

| Rol | Nombre | Responsabilidad |
|-----|--------|-----------------|
| Product Owner | [NOMBRE] | Decisiones de producto |
| Tech Lead | [NOMBRE] | Decisiones técnicas |
| Project Manager | [NOMBRE] | Seguimiento del plan |

---

## 10. DIMENSIONAMIENTO TÉCNICO

### 10.1 Estimación de Esfuerzo

| Actividad | HH Estimadas |
|-----------|--------------|
| Análisis y diseño | [HH] |
| Desarrollo backend | [HH] |
| Desarrollo frontend | [HH] |
| Integración | [HH] |
| QA | [HH] |
| Documentación | [HH] |
| Gestión de proyecto | [HH] |
| **TOTAL** | **[TOTAL]** |

### 10.2 Recursos Humanos
- **Personas:** [N]
- **Duración:** [SEMANAS] semanas
- **Carga promedio:** [HH/SEMANA] horas/semana

---

## 11. MODELO ECONÓMICO

### 11.1 Tipo
- **Modelo:** Proyecto de Alcance Definido (Fixed Scope)

### 11.2 Cálculo

| Concepto | Valor |
|----------|-------|
| Horas totales | [HH] |
| Tarifa promedio | [TARIFA] USD/HH |
| Subtotal servicios | [SUBTOTAL] |
| Licencias (si aplica) | [LICENCIAS] |
| Infraestructura (1 mes) | [INFRA] |
| **TOTAL PROYECTO** | **[TOTAL]** |

### 11.3 Forma de Pago
- [ESTRUCTURA_PAGO]

---

## 12. RIESGOS Y MITIGACIÓN

| Riesgo | Probabilidad | Impacto | Mitigación |
|--------|-------------|--------|-----------|
| [RISK1] | Baja | Alto | [MIT1] |
| [RISK2] | Media | Medio | [MIT2] |
| [RISK3] | Alta | Bajo | [MIT3] |

---

## 13. CRITERIOS DE ÉXITO

- [ ] Todas las RF implementadas
- [ ] Testing pasa 95%+
- [ ] Usuarios entrenados
- [ ] Documentación completa
- [ ] Sistema estable en producción

---

## 14. SUPUESTOS

- [SUP1]
- [SUP2]
- [SUP3]
- [SUP4]

---

## 15. EXCLUSIONES

- [EXC1]
- [EXC2]
- [EXC3]

---

## 16. DEPENDENCIAS

**Del cliente:**
- [DEP1]
- [DEP2]

**Externas:**
- [DEP3]

---

## 17. OBSERVACIONES

[NOTAS_CONSULTOR]

---

## 18. RESUMEN PARA STAKEHOLDERS

**Problema:**
[PROBLEMA_SÍNTESIS]

**Solución:**
[SOLUCIÓN_SÍNTESIS]

**Deliverables:**
- Análisis + diseño
- Sistema funcional integrado
- Ambiente productivo
- Equipo entrenado
- Documentación técnica

**Inversión:**
[TOTAL] USD en [DURACIÓN]

**Timeline:**
[DIAGRAMA_GANTT_SIMPLIFICADO]

**Recomendación:**
[RECOMENDACIÓN]

---

**Documento generado:** [FECHA_HOY]  
**Vigencia:** [DÍAS] días desde emisión  
**Próxima reunión:** [FECHA_PROXIMA]
