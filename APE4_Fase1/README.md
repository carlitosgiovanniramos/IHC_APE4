# APE 4 · Fase 1 — De los requisitos a la arquitectura de información, navegación y wireframes

**Asignatura:** Interacción Humano-Computador · **Docente:** Ing. Mg. José Caiza · **Nivel:** Quinto – A · UTA FISEI · Julio – diciembre 2026

**Caso:** CaféU, aplicación de pedidos de la cafetería universitaria (taller «¿Confirmar o editar?» trabajado en clase).

**Autor:** Carlos Giovanni Ramos Jácome ([@carlitosgiovanniramos](https://github.com/carlitosgiovanniramos)) — práctica individual.

## Proceso

Requisito → Pantalla → Sitemap → User flow → Componentes → Wireframe

## Entregables

| N.º | Entregable | Archivo |
|---|---|---|
| 1 | Matriz de requisitos y pantallas | [01_matriz_requisitos_pantallas.md](01_matriz_requisitos_pantallas.md) |
| 2 | Sitemap del proyecto | [02_sitemap.png](02_sitemap.png) |
| 3 | Dos diagramas user flow | [03_userflow_1_realizar_pedido.png](03_userflow_1_realizar_pedido.png) · [03_userflow_2_modificar_pedido.png](03_userflow_2_modificar_pedido.png) |
| 4 | Esquema de navegación e inventario de componentes | [04_esquema_navegacion.png](04_esquema_navegacion.png) · [04_navegacion_e_inventario_componentes.md](04_navegacion_e_inventario_componentes.md) |
| 5 | Wireframes de baja fidelidad (7 pantallas + 4 estados) | [05_wireframes/](05_wireframes/) |
| 6 | Documento PDF con la explicación didáctica | [06_documento/APE4_Fase1_CafeU.pdf](06_documento/APE4_Fase1_CafeU.pdf) · [06_documento/APE4_Fase1_CafeU.docx](06_documento/APE4_Fase1_CafeU.docx) |
| 7 | Prototipo | Prototipo HTML navegable (W1 – W7, E1 – E4): [07_prototipo/index.html](07_prototipo/index.html) · En vivo: https://carlitosgiovanniramos.github.io/IHC_APE4/APE4_Fase1/07_prototipo/ · Wireflow del taller en Figma: https://flap-bottom-98029162.figma.site/ |
| 8 | Protocolo de validación y casos de prueba | [08_protocolo_pruebas_usabilidad.md](08_protocolo_pruebas_usabilidad.md) |

## Wireframes

Los wireframes tienen formato de aplicación web móvil: marco de celular, barra de pestañas inferior (Inicio, Menú, Mis pedidos, Mi pedido · n), menú en cuadrícula de dos columnas, botones en forma de píldora y confirmaciones en hoja inferior. Se generan desde el prototipo HTML, por lo que ambos coinciden.

| Código | Pantalla | Origen |
|---|---|---|
| W1 | Inicio | Prototipo HTML |
| W2 | Menú | Prototipo HTML |
| W3 | Detalle del producto | Prototipo HTML |
| W4 | Resumen del pedido | Pantalla 1 del taller (Figma) |
| W5 | Modificar pedido | Pantalla 2B del taller (Figma) |
| W6 | Confirmación de compra | Pantalla 2A del taller (Figma) |
| W7 | Estado del pedido | Prototipo HTML |
| E1 – E4 | Pago rechazado, pedido vacío, producto agotado, confirmar eliminación | Prototipo HTML |

`05_wireframes/00_taller_wireflow_figma.png` es el wireflow original del taller en Figma.

## Cómo usar el prototipo

Abrir `07_prototipo/index.html` en el navegador (no necesita internet) o la versión publicada en GitHub Pages. El panel lateral permite simular un pago rechazado y reiniciar. Tareas sugeridas:

1. Pedir un Café Americano y un Sánduche, confirmarlos y consultar el estado del pedido.
2. Antes de pagar, quitar el sánduche, subir el café a 2 y guardar los cambios.
