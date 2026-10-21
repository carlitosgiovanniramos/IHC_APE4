# 01 · Matriz de requisitos, usuarios y pantallas — CaféU

## Usuarios

| Usuario | Descripción y contexto | Necesidades | Tipo |
|---|---|---|---|
| Estudiante universitario | Compra entre clases, con poco tiempo y desde el celular o el navegador; la cafetería suele estar llena. | Ver qué hay y cuánto cuesta; armar el pedido sin explicarlo en caja; revisarlo y corregirlo antes de pagar; saber cuándo retirarlo. | Principal (usa todas las pantallas) |
| Personal de la cafetería | Prepara y entrega los pedidos en el edificio central. | Recibir pedidos claros y pagados, identificados por un número que el estudiante presenta al retirar. | Secundario (recibe el resultado del flujo; su panel queda fuera del alcance) |

## Funcionalidades principales

| N.º | Funcionalidad principal | Requisitos que agrupa | Pantallas |
|---|---|---|---|
| F1 | Consultar el menú y armar el pedido | RF-01, RF-02, RF-03 | W1, W2, W3 |
| F2 | Revisar, confirmar y pagar el pedido | RF-04, RF-06, RF-07 | W4, W6 |
| F3 | Modificar el pedido antes de pagar | RF-05 | W5 (regresa a W4) |
| F4 | Consultar el estado del pedido | RF-08 | W7 |

## Matriz de requisitos y pantallas

| Código | Requisito funcional | Usuario · necesidad | Pantalla(s) | Prioridad |
|---|---|---|---|---|
| RF-01 | Mostrar el menú del día con nombre, descripción, precio y disponibilidad de cada producto. | Estudiante · saber qué hay y cuánto cuesta | W1 Inicio, W2 Menú | Alta |
| RF-02 | Buscar productos y filtrarlos por categoría (Todo, Bebidas, Comida). | Estudiante · encontrar rápido lo que quiere | W2 Menú | Media |
| RF-03 | Ver el detalle de un producto, elegir opción y cantidad, y agregarlo al pedido. | Estudiante · armar el pedido sin explicarlo en caja | W3 Detalle | Alta |
| RF-04 | Mostrar el resumen del pedido: productos, cantidades, precios, total, lugar de retiro y método de pago. | Estudiante · revisar antes de pagar | W4 Resumen | Alta |
| RF-05 | Modificar cantidades y eliminar productos, recalculando el total, y guardar o descartar los cambios. | Estudiante · corregir un error a último momento | W5 Modificar | Alta |
| RF-06 | Confirmar y pagar el pedido, informando si el pago fue rechazado sin perder el pedido. | Estudiante · pagar con seguridad | W4 → W6 | Alta |
| RF-07 | Mostrar la confirmación con número de pedido, tiempo estimado y resumen de lo pagado. | Estudiante y personal · identificar el pedido al retirar | W6 Confirmación | Alta |
| RF-08 | Consultar el estado del pedido en curso (recibido, en preparación, listo) y el historial. | Estudiante · saber cuándo retirar | W7 Estado del pedido | Media |
