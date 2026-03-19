# MCP: Sales

## Descripción

Módulo encargado de consultar y procesar información de ventas desde la base de datos en Supabase.

Este MCP permite al sistema entender qué productos se venden más, detectar patrones de compra y generar inteligencia comercial.

---

## Función

- Consultar historial de ventas
- Identificar productos más vendidos
- Analizar comportamiento por ciudad
- Detectar tendencias de compra

---

## Datos disponibles

- ID de venta
- Teléfono del cliente
- ID del producto
- Cantidad
- Valor total
- Ciudad
- Fecha de compra

---

## Uso en el sistema

Este MCP se utiliza en:

- Recomendación de productos (basado en popularidad)
- Estrategias de venta
- Fases futuras de analítica avanzada
- Optimización del catálogo

---

## Ejemplo de consulta

Productos más vendidos:

GET /sales?select=product_id,count:count(product_id)&order=count.desc

---

Ventas por ciudad:

GET /sales?select=city,sum:sum(total_amount)&group=city

---

## Ejemplo de respuesta

```json
[
  {
    "product_id": "uuid123",
    "count": 45
  },
  {
    "product_id": "uuid456",
    "count": 30
  }
]
