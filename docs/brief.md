# Autonomous Sales System

## 🧾 Resumen Ejecutivo

Autonomous Sales System es una solución basada en inteligencia artificial diseñada para automatizar y optimizar la atención al cliente en WhatsApp.

El sistema busca transformar un proceso manual en un sistema autónomo capaz de responder, recomendar productos y mejorar la conversión de ventas.

---

## 🚨 Problema

El negocio actualmente presenta:

- Alto volumen de chats manuales
- Falta de seguimiento a clientes
- No se aprovechan los datos de ventas
- Respuestas inconsistentes
- Subutilización de más de 7,000 clientes y 2,000 productos activos

---

## 🎯 Objetivos

- Automatizar la atención inicial
- Mejorar la conversión
- Recomendar productos de forma inteligente
- Reducir carga operativa
- Sentar bases para analítica futura

---

## 🧠 Solución

Sistema multi-agente compuesto por:

- Orchestrator (n8n)
- Agente de ventas
- Subagent clasificador
- MCP de productos

---

## 🏗️ Arquitectura

- Entrada: WhatsApp API
- Procesamiento: n8n
- Decisión: Clasificador
- Acción: Skills
- Datos: Supabase

---

## ⚙️ Componentes

### Reglas
- Tono comercial
- Enfoque en cierre

### Skills
- Responder cliente
- Recomendar producto
- Cerrar venta

### MCP
- Productos
- Clientes
  
### SubAgent
- Clasificación de intención

---

## 🌐 Servicios

- n8n
- Supabase
- WhatsApp API
- IA (LLM)

---

## 📊 Datos

Se utiliza Supabase con carga por archivos CSV para:

- Productos
- Clientes
- Ventas
