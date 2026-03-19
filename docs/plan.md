# Plan de Implementación – Autonomous Sales System

## 🎯 Enfoque

Se desarrollará un MVP funcional priorizando ejecución sobre complejidad.

---

## 🔹 Fase 1: MVP Conversacional

### Objetivo
Automatizar la atención inicial y recomendación de productos.

---

### Componentes

- Orchestrator (n8n)
- Clasificador de intención
- Skills:
  - Responder cliente
  - Cerrar venta
- MCP de productos (Supabase)

---

### Flujo

1. Cliente escribe
2. Clasificador analiza intención
3. Orchestrator decide acción
4. Se ejecuta skill
5. Se consulta base de datos
6. Se responde

---

### Resultado

- Automatización básica
- Respuestas consistentes
- Reducción de carga manual

---

## 🔹 Fase 2: Clientes

- Perfilamiento
- Segmentación
- Reactivación

---

## 🔹 Fase 3: Analítica

- Productos más vendidos
- Insights por ciudad
- Optimización comercial

---

## 🚧 Tecnologías

- n8n
- Supabase
- WhatsApp API
- IA
