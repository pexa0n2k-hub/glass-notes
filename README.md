# Glass Notes V2.1 — Arquitectura Segura

V2.1 mantiene el estilo Liquid Glass de V2.0 y se enfoca en proteger los datos y facilitar futuras actualizaciones.

## Seguridad de datos
- Esquema de datos versionado (`schema: 3`).
- Normalización y validación al cargar.
- Migración básica desde `glass_notes_v03`.
- Respaldo local anterior a cada guardado.
- Recuperación desde respaldo local.
- Exportación/importación JSON.
- Fallos de render no bloquean toda la aplicación.

## Funciones conservadas
Notas, pendientes con checkbox, pagos, JARVIS por texto/voz cuando el navegador lo soporta y fondo personalizable.

## Publicación
Sube `index.html`, `manifest.json`, `sw.js` y `README.md` a la raíz de `main` en GitHub Pages.


## V2.1.1 — Pagos corregidos
El módulo de pagos ahora incluye fecha, hora, vencimiento, estado, edición, marcado como pagado y totales separados. Los registros existentes se migran sin eliminar los campos que ya tengan.
