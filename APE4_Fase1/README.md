# APE 4 · Fase 1 — De los requisitos a la arquitectura de información, navegación y wireframes

**Asignatura:** Interacción Humano-Computador · **Docente:** Ing. Mg. José Caiza · **Nivel:** Quinto – A · UTA FISEI · Julio – diciembre 2026

**Caso:** CaféU, aplicación de pedidos de la cafetería universitaria (taller «¿Confirmar o editar?» trabajado en clase).

**Integrantes y Roles Oficiales:**
- **Alison Marcela Cobos Taco** ([@Itsuna18](https://github.com/Itsuna18)) — *Desarrollador Back-End* (API, modelos, persistencia, endpoints)
- **Melany Saleth Cevallos Goyes** ([@SalyC15](https://github.com/SalyC15)) — *Desarrollador Front-End* (Vistas, componentes UI, diseño, wizard)
- **Carlos Giovanni Ramos Jácome** ([@carlitosgiovanniramos](https://github.com/carlitosgiovanniramos)) — *Tester* (Protocolos de validación, casos de prueba, métricas SUS)
- **Henry Daniel Lagua Flores** ([@Hlagua](https://github.com/Hlagua)) — *QA / Arquitecto* (Arquitectura de información, sitemap, revisión e informe final)

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
| 7 | Prototipo | Figma (W1 – W7, E1 – E4, navegable): https://www.figma.com/proto/0bxGDlHenLKFwC9IroyRXt?node-id=2-4&starting-point-node-id=2%3A4 · Wireflow del taller: https://flap-bottom-98029162.figma.site/ · Prototipo HTML: [07_prototipo/index.html](07_prototipo/index.html) · En vivo: https://hlagua.github.io/APE4_Fase1/ |
| 8 | Protocolo de validación y casos de prueba | [08_protocolo_pruebas_usabilidad.md](08_protocolo_pruebas_usabilidad.md) |

## Wireframes

| Código | Pantalla | Origen |
|---|---|---|
| W1 | Inicio | Figma y prototipo HTML |
| W2 | Menú | Figma y prototipo HTML |
| W3 | Detalle del producto | Figma y prototipo HTML |
| W4 | Resumen del pedido | Pantalla 1 del taller (Figma) |
| W5 | Modificar pedido | Pantalla 2B del taller (Figma) |
| W6 | Confirmación de compra | Pantalla 2A del taller (Figma) |
| W7 | Estado del pedido | Figma y prototipo HTML |
| E1 – E4 | Pago rechazado, pedido vacío, producto agotado, confirmar eliminación | Figma y prototipo HTML |
| W4b, W5b | Resumen actualizado y modificar con cambios | Solo Figma (completan el flujo 2) |

`05_wireframes/00_taller_wireflow_figma.png` es el wireflow original del taller en Figma.

## Cómo usar el prototipo

**En Figma:** abrir el archivo, pulsar *Presentar* (▶) y elegir un flujo: «Flujo 1 · Realizar y confirmar un pedido», «Flujo 2 · Modificar el pedido antes de pagar» o «Estado · Pago rechazado». Todos los botones y enlaces están conectados.

**En HTML:** abrir `07_prototipo/index.html` en el navegador (no necesita internet). El panel lateral permite simular un pago rechazado y reiniciar. Tareas sugeridas:

1. Pedir un Café Americano y un Sánduche, confirmarlos y consultar el estado del pedido.
2. Antes de pagar, quitar el sánduche, subir el café a 2 y guardar los cambios.
