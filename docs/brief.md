# Autonomous Sales System

## 🧾 Resumen Ejecutivo

Autonomous Sales System es una solución basada en agentes de inteligencia artificial diseñada para automatizar, optimizar y escalar el proceso de atención y ventas en WhatsApp.

El sistema transforma un modelo manual y reactivo en una arquitectura autónoma capaz de responder clientes, recomendar productos y generar inteligencia comercial basada en datos.

---

## 🚨 Problema

El proceso comercial actual presenta limitaciones estructurales que afectan la escalabilidad y eficiencia del negocio:

- Alto volumen de conversaciones gestionadas manualmente
- Falta de consistencia en respuestas comerciales
- Ausencia de seguimiento a clientes
- Subutilización de datos históricos
- No existe analítica estructurada para toma de decisiones

### 📊 Contexto del negocio

- Base de clientes: 7.000
- Productos activos: 2.000
- Conversaciones diarias: entre 100 y 500
- Canales principales: WhatsApp

Estas condiciones generan dependencia operativa del equipo humano y limitan el crecimiento.

---

## 🎯 Objetivos del Sistema

### Objetivo general
Diseñar un sistema autónomo basado en agentes que permita escalar el proceso comercial mediante automatización inteligente.

### Objetivos específicos

- Automatizar la atención inicial de clientes
- Mejorar la tasa de conversión
- Recomendar productos de forma contextual
- Reducir carga operativa del equipo humano
- Habilitar el uso de datos para decisiones comerciales
- Sentar bases para analítica y reactivación de clientes

---

## 🧠 Solución Propuesta

Se propone una arquitectura multi-agente compuesta por:

### 🔹 Orchestrator
Coordina el flujo de decisiones del sistema y gestiona la interacción entre componentes.

### 🔹 Sales Agent
Encargado de la comunicación con el cliente y la generación de respuestas orientadas a la venta.

### 🔹 SubAgent Clasificador
Analiza los mensajes y detecta intención y categoría.

### 🔹 MCPs (Model Context Protocols)
Permiten el acceso estructurado a datos externos:

- Productos
- Clientes
- Ventas

---

## 🏗️ Arquitectura de Alto Nivel

### Flujo general

1. Cliente envía mensaje por WhatsApp
2. Orchestrator recibe el mensaje (n8n)
3. Clasificador analiza intención
4. Se selecciona el skill adecuado
5. Se consultan datos (MCP)
6. Se genera respuesta
7. Se envía al cliente

---

## ⚙️ Componentes del Sistema

### 🧩 Reglas

- Mantener tono comercial y cercano
- Priorizar conversión
- Evitar respuestas ambiguas
- Guiar la conversación hacia acción

---

### ⚡ Skills

- Responder cliente
- Recomendar productos
- Cerrar venta

---

### 🌐 MCPs

- MCP Productos → consulta catálogo
- MCP Clientes → personalización
- MCP Ventas → inteligencia comercial

---

### 🤖 SubAgents

- Clasificador de intención y categoría

---

## 🌐 Servicios y Tecnologías

- n8n → Orquestación de flujos
- Supabase → Base de datos externa
- WhatsApp API → Canal de comunicación
- Modelo de lenguaje (LLM) → Procesamiento de lenguaje natural

---

## 📊 Estrategia de Datos

El sistema utiliza una base de datos externa en Supabase alimentada mediante cargas masivas (CSV).

### Datos gestionados:

- Productos
- Clientes
- Ventas
- Conversaciones

### Ventajas:

- Independencia del sistema principal
- Mayor control y limpieza de datos
- Optimización para uso con IA
- Iteración rápida durante desarrollo

---

## 🚀 Alcance Inicial (MVP)

El MVP incluye:

- Automatización de atención inicial
- Clasificación de intención
- Recomendación básica de productos
- Flujo funcional en n8n

---

## 🔮 Evolución del Sistema

El sistema está diseñado para evolucionar hacia:

- Perfilamiento avanzado de clientes
- Reactivación automática
- Analítica de ventas
- Recomendaciones predictivas

---

## 💡 Impacto Esperado

La implementación del sistema permitirá:

- Escalar la atención sin aumentar el equipo
- Incrementar la tasa de conversión
- Aprovechar datos existentes
- Automatizar procesos comerciales clave
- Construir una base de inteligencia de negocio

---
