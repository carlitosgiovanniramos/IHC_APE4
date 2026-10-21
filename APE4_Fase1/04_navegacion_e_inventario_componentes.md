# 04 · Esquema de navegación e inventario de componentes — CaféU

![Esquema de navegación](04_esquema_navegacion.png)

## Menú principal y mecanismos de navegación

Como el estudiante pide sobre todo desde el celular, el menú principal es una barra de pestañas inferior (Inicio, Menú, Mis pedidos y «Mi pedido · n»), en la zona que alcanza el pulgar. La marca CaféU se mantiene en la barra superior y lleva a Inicio.

| Mecanismo | Dónde aparece | Función | Por qué facilita la interacción |
|---|---|---|---|
| Barra de pestañas inferior (Inicio · Menú · Mis pedidos · Mi pedido · n) y marca CaféU en la parte superior | W1, W2, W7 | Acceso directo a las secciones de nivel 1. | Siempre visible, en el mismo lugar y al alcance del pulgar (ley de Fitts); el contador de «Mi pedido» muestra el estado del pedido sin abrirlo. |
| Botón «←» en el encabezado | W3, W4, W5 | Volver a la pantalla anterior. | Salida clara en el flujo de compra; en W5 pregunta antes de descartar cambios. |
| Botón principal (relleno) | Todas | La acción esperada: «Ver menú», «Agregar al pedido», «Confirmar y Pagar», «Guardar Cambios», «Ver Estado del Pedido». | Una sola acción destacada por pantalla reduce la duda sobre qué hacer (ley de Hick). |
| Botón secundario (borde) | W2, W4, W7 | Alternativas: «Ver detalle», «Editar Pedido», «Volver al menú». | Diferencia visual entre la acción principal y la alternativa. |
| Barra fija «Ver mi pedido» | W2 (con productos) | Llevar al resumen sin buscar el botón. | Muestra cantidad y total mientras se sigue comprando; queda justo encima de la barra de pestañas. |
| Enlace «Volver al inicio» | W6 | Cerrar el flujo de compra. | Evita callejones sin salida después de pagar. |
| Flujo de compra enfocado | W4, W5, W6 | Oculta la barra de pestañas durante la revisión y el pago. | Menos distracciones y menos riesgo de abandonar el pedido a medio camino. |

## Inventario de componentes reutilizables

| Componente | Descripción | Pantallas | Principio aplicado |
|---|---|---|---|
| Barra de pestañas | Cuatro pestañas con icono y texto; «Mi pedido · n» lleva un contador. La marca va en la barra superior. | W1, W2, W7 | Consistencia; visibilidad del estado |
| Encabezado con «←» | Botón circular «←» y título alineado a la izquierda. | W3, W4, W5 | Control y libertad del usuario |
| Botón principal / secundario | Forma de píldora: relleno oscuro para la acción esperada, borde para la alternativa y gris si está desactivado. En el flujo de compra van apilados y a todo el ancho. | Todas | Jerarquía visual; prevención de errores |
| Campo de búsqueda | Entrada redondeada con icono de lupa e indicación «Buscar producto…». | W2 | Reconocer antes que recordar |
| Filtros (chips) | Todo · Bebidas · Comida; el activo va relleno. | W2 | Reducción de la carga cognitiva |
| Tarjeta de producto | Mosaico en cuadrícula de dos columnas: imagen, nombre, descripción, precio, etiqueta «AGOTADO» y «Ver detalle». | W2 | Agrupación (proximidad) |
| Tarjeta de resumen | Lista de productos con cantidad y precio, y total en negrita. | W4, W6 | Visibilidad del estado |
| Selector de cantidad | Botones circulares «−» número «+», con áreas táctiles de 36 px o más. | W3, W5 | Ley de Fitts; prevención de errores (mínimo 1) |
| Icono de basurero | Elimina un producto del pedido. | W5 | Control del usuario |
| Diálogo de confirmación (hoja inferior) | Hoja inferior con «¿Eliminar…?» o «¿Descartar los cambios?», la acción y «Cancelar» apilados al alcance del pulgar. | W5 | Prevención de errores |
| Mensaje de estado | Éxito (✓), error (!) y vacío, con texto y una salida. | W3, W4, W5, W6 | Ayuda a reconocer y recuperarse de errores |
| Indicador de pasos | Línea de tiempo vertical: Recibido → En preparación → Listo para retirar, con el detalle de cada paso. | W7 | Visibilidad del estado del sistema |
| Aviso emergente (toast) | «Agregado a tu pedido», «Cambios guardados». | W2, W4 | Retroalimentación inmediata |
