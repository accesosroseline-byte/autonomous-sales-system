architecture/system.md

# System Design

## Flujo principal

1. Usuario envía mensaje por WhatsApp
2. n8n recibe el mensaje (Webhook)
3. Clasificador detecta intención
4. Orchestrator decide acción
5. Se ejecuta skill
6. Se consulta Supabase (si aplica)
7. Se responde al cliente

## Componentes

- Orchestrator: n8n
- AI: modelo de lenguaje
- Data: Supabase
- Canal: WhatsApp API
