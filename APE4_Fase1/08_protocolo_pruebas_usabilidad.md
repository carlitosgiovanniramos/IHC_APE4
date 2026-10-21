# 08 · Protocolo de Validación y Casos de Prueba de Usabilidad — CaféU

**Autor:** Carlos Giovanni Ramos Jácome (@carlitosgiovanniramos)  
**Proyecto:** APE 4 · Fase 1 — CaféU (IHC - FISEI - UTA)

---

## 1. Objetivo del Protocolo de Pruebas

Verificar que la arquitectura de información, los wireflows y el prototipo interactivo de **CaféU** cumplan con los principios de usabilidad, prevención de errores y control del usuario, permitiendo a los estudiantes completar sus pedidos de forma ágil, segura y sin fricciones cognitivas.

---

## 2. Casos de Prueba de Usabilidad Diseñados

| Código | Tarea / Caso de Prueba | Precondición | Pasos de Ejecución | Resultado Esperado | Criterio de Aceptación |
|---|---|---|---|---|---|
| **CP-01** | **Búsqueda y filtrado en el menú** | Estudiante en pantalla Inicio (W1). | 1. Presionar «Ver Menú».<br>2. Aplicar filtro «Bebidas».<br>3. Ingresar «Café» en el buscador. | Se listan únicamente bebidas coincidentes; los productos agotados muestran la etiqueta «AGOTADO» y, al abrir su detalle (E3), no permiten agregarlos al pedido. | Reconocimiento visual inmediato, sin resultados engañosos. |
| **CP-02** | **Flujo completo de realización de pedido (Happy Path)** | Estudiante en Menú (W2). | 1. Seleccionar *Café Americano* ($1.50) y agregarlo.<br>2. Seleccionar *Sánduche* de jamón y queso ($2.75) y agregarlo.<br>3. Abrir «Ver mi pedido» (W4).<br>4. Presionar «Confirmar y Pagar». | Se muestra la pantalla de Confirmación (W6) con «Pago aprobado», número de pedido #A24, tiempo estimado (10 min) y resumen de lo pagado ($4.25). | El pedido se procesa en menos de 4 pasos clave sin callejones sin salida. |
| **CP-03** | **Modificación del pedido antes de pagar** | Pedido armado en pantalla Resumen (W4). | 1. Presionar «Editar Pedido» (W5).<br>2. Pulsar «+» en el Café Americano para subir a 2.<br>3. Pulsar el icono de basurero en el Sánduche.<br>4. Confirmar eliminación en la hoja inferior (E4).<br>5. Presionar «Guardar Cambios». | El subtotal se recalcula en tiempo real a $3.00. Al guardar cambios, el resumen W4 refleja exactamente 2 cafés y ningún sánduche. | El usuario mantiene control total para rectificar errores antes de pagar (heurística de libertad y control). |
| **CP-04** | **Resiliencia ante fallo de pago (Pago Rechazado)** | Pedido listo en Resumen (W4) con simulador activado. | 1. En el panel de simulación lateral, activar «Simular pago rechazado».<br>2. Presionar «Confirmar y Pagar». | Aparece el estado de error E1 con mensaje constructivo. El carrito NO se vacía; se permite reintentar el pago o cambiar de método. | Prevención y recuperación amigable de errores sin pérdida de datos. |
| **CP-05** | **Monitoreo y consulta de estado del pedido** | Pedido confirmado (#A24). | 1. Desde W6 presionar «Ver Estado del Pedido» (W7).<br>2. Observar la línea de tiempo de etapas. | Se evidencia claramente la transición visual: Recibido → En preparación → Listo para retirar en el Edificio Central. | Visibilidad permanente del estado del sistema (Heurística #1 de Nielsen). |

---

## 3. Matriz de Heurísticas de Usabilidad Verificadas (Jakob Nielsen)

| Heurística | Componente / Pantalla Verificada | Evidencia en el Prototipo CaféU |
|---|---|---|
| **H1: Visibilidad del estado** | Barra de pestañas inferior (W1, W2, W7) y línea de tiempo (W7) | El contador de la pestaña «Mi pedido · n» actualiza la cantidad de ítems en vivo. La línea de tiempo vertical indica el avance de preparación. |
| **H2: Correspondencia con el mundo real** | Menú, productos, cantidades e iconos | Uso de terminología cotidiana de cafetería, iconos estándar (basurero, flecha atrás, marca de verificación ✓). |
| **H3: Control y libertad del usuario** | Modificar pedido (W5) y botón «←» | El usuario puede salir en cualquier momento, modificar cantidades o cancelar la edición con confirmación de descarte. |
| **H4: Consistencia y estándares** | Sistema de botones y encabezados | Botones primarios en fondo sólido oscuro para la acción recomendada; botones secundarios con borde; estilo consistente en todas las vistas. |
| **H5: Prevención de errores** | Hoja inferior de confirmación E4 y selector de cantidad | Se solicita confirmación antes de eliminar un ítem del pedido; el selector de cantidad no permite bajar de 1. |
| **H6: Reconocimiento antes que recuerdo** | Tarjeta de resumen (W4) y filtros (W2) | Se muestra el desglose completo de productos, precios y totales sin exigir que el estudiante memorice lo seleccionado. |
| **H9: Ayuda a diagnosticar y recuperarse de errores** | Pantalla E1 (Pago rechazado) | Explica la causa del fallo y proporciona una salida directa («Reintentar pago») conservando los datos del pedido intactos. |

---

## 4. Métricas de Evaluación Previstas (SUS y SEQ)

- **System Usability Scale (SUS):** Meta establecida $\ge 85/100$ (Grado A, Usabilidad Excelente).
- **Single Ease Question (SEQ):** Escala de 1 a 7 al completar la tarea de modificación del pedido; meta promedio $\ge 6.5/7$.
- **Tasa de éxito de tareas:** 100% en las 3 tareas fundamentales del prototipo.
