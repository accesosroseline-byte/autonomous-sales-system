# MCP: Customers

## Descripción

Módulo encargado de consultar información de clientes desde la base de datos en Supabase.

Este MCP permite que el sistema tenga contexto sobre quién es el cliente y su historial, habilitando respuestas más personalizadas y estratégicas.

---

## Función

- Consultar cliente por número de teléfono
- Obtener historial básico de compras
- Identificar tipo de cliente
- Proveer datos para personalización de respuestas

---

## Datos disponibles

- Nombre
- Teléfono
- Ciudad
- Total de compras
- Fecha de última compra

---

## Uso en el sistema

Este MCP se utiliza en:

- Personalización de respuestas
- Recomendación de productos
- Estrategias de cierre de venta
- Fases futuras de reactivación de clientes

---

## Ejemplo de consulta

Buscar cliente por teléfono:

GET /customers?phone=eq.3001234567

---

## Ejemplo de respuesta

```json
{
  "name": "Maria Lopez",
  "city": "Medellin",
  "total_purchases": 120000,
  "last_purchase_date": "2026-02-10"
}
