# Costos de Proyectos

App web para el celular que calcula costos de materiales y lleva el registro de gastos de cada proyecto (una casa, un local, un cerramiento…).

## Qué hace

- **Inicio:** balance del mes de todos los proyectos (por proyecto y por categoría), con meses anteriores y exportación a CSV.
- **Proyectos:** lista compacta; toca un proyecto para abrirlo y el lápiz para editarlo. Cada proyecto tiene su resumen (presupuesto fijo o por proformas aceptadas, disponible, gasto por mes), precios, proformas, gastos y etapas.
- **Etapas:** divide un proyecto en las fases que tú definas y sigue el avance de cada etapa contra su presupuesto. Avisa si lo comprado no cuadra con la proforma.
- **Precios:** lista de materiales y servicios con unidad y precio unitario. Puedes copiar la lista de otro proyecto.
- **Proforma:** eliges materiales, ajustas cantidades con − y + y la app calcula el subtotal, el IVA (opcional, 15 % por defecto) y el total. Se puede **aceptar** (pasa a ser presupuesto) y **marcar como pagada**, en uno o varios pagos que se suman a los gastos. Se comparte por WhatsApp o se descarga en PDF o CSV.
- **Gastos:** registro rápido con teclado numérico, fecha de hoy por defecto, categoría, etapa, proveedor y foto de la factura. Se agrupa por mes.

## Cómo usarla

Ábrela desde GitHub Pages en Chrome (Android) y, en el menú ⋮, elige **Agregar a pantalla principal** o **Instalar app**. Después abre como una app normal, incluso sin internet.

## Dónde se guardan los datos

En esta versión los datos quedan **solo en el navegador del teléfono** (localStorage). Desde la pantalla **Proyectos** puedes descargar un respaldo (archivo `.json`) e importarlo en otro teléfono o navegador. Si borras los datos de Chrome sin respaldo, se pierden. Las fotos de facturas se guardan en el teléfono y no van en el respaldo.

La descarga en PDF necesita internet la primera vez (usa la librería jsPDF).

## Archivos

- `index.html` — toda la app (HTML, CSS y JavaScript en un solo archivo; jsPDF se carga solo al descargar un PDF).
- `sw.js` — permite abrirla sin conexión.
- `manifest.webmanifest`, `icon*.png`, `icon.svg` — instalación en la pantalla principal.

Moneda: dólares (USD).
