# Orchestrator Agent

## Descripción

El Orchestrator es el agente principal del sistema. Su función es recibir los mensajes de los clientes y coordinar la ejecución de los diferentes componentes del sistema.

---

## Responsabilidades

- Recibir mensajes desde WhatsApp
- Enviar mensaje al clasificador
- Interpretar la intención del cliente
- Decidir qué skill ejecutar
- Coordinar el acceso a datos (MCP)
- Retornar la respuesta final

---

## Flujo

1. Recibe mensaje del cliente
2. Envía mensaje al SubAgent clasificador
3. Analiza intención detectada
4. Selecciona skill correspondiente:
   - responder_cliente
   - recomendar_producto
   - cerrar_venta
5. Ejecuta la acción
6. Retorna respuesta

---

## Decisiones clave

- Si intención = saludo → responder_cliente
- Si intención = compra → recomendar_producto
- Si intención = cierre → cerrar_venta

---

## Tecnologías

- n8n (orquestación)
- API WhatsApp
- Modelo de lenguaje (IA)
