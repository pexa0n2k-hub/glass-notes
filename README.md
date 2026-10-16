# Glass Notes V3.4.4 — Pagos separados

## Corrección
- La pantalla principal de Pagos usa las pestañas Pendientes y Liquidados.
- Se retiró la reinserción del módulo antiguo Centro de Pagos que podía volver a mezclar la vista.
- Se conservó el almacenamiento existente, el marcado como pagado, la edición/eliminación y la lógica de recurrencias.
- Se incrementó la versión de caché del Service Worker para forzar que la PWA actualice `index.html` en GitHub Pages.

## Cómo subirlo
Extrae el ZIP y sube `index.html`, `sw.js` y `manifest.json` a la raíz del repositorio, reemplazando los archivos existentes. No subas los archivos dentro de una subcarpeta.

Después de subirlos, abre la web de GitHub Pages en Chrome, recarga y si la app instalada sigue mostrando lo anterior, cierra la PWA y vuelve a abrirla tras unos segundos para que se active el nuevo Service Worker. No borres los datos del sitio.
