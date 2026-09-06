# Glass Notes V2.0 — Stable

Esta versión reemplaza el núcleo que estaba provocando el mensaje **“dato o función incompatible”**.

## Cambios principales
- Almacenamiento local protegido con validación.
- Si un dato guardado está corrupto, la interfaz no se cae.
- Notas, pendientes y pagos.
- Casillas para tachar pendientes y sección de completados.
- JARVIS con comandos de texto y reconocimiento de voz cuando el navegador lo permite.
- Fondo de pantalla desde URL o galería.
- Color de acento personalizable.
- Respaldo y restauración JSON.
- Service Worker nuevo con caché independiente.

## Archivos
- `index.html`
- `manifest.json`
- `sw.js`

## Instalación en GitHub Pages
Sube los tres archivos a la raíz de la rama `main`. GitHub Pages debe publicar `/ (root)` desde `main`.

Después de publicar, abre la página y haz una recarga completa. Si el navegador conserva el Service Worker anterior, borra los datos/caché del sitio una vez y vuelve a abrirlo.


## V2.0.1 — Pagos
Corrección aislada del módulo de pagos: fecha, hora, vencimiento, estado, edición y totales. Notas y listas parten directamente de V2.0 Stable.


## V2.0.2 — Cierre de ventanas
Corrección puntual del botón X: se renombró la función de cierre para evitar conflicto con la API `window.close()` del navegador. También se actualizó el caché del Service Worker.


## V2.0.3 — Fondo personalizado
Corrección del fondo desde galería y caché actualizado.


## V2.0.4 — Gestos
En notas, listas y pagos: deslizar de izquierda a derecha abre modificación; deslizar de derecha a izquierda solicita confirmación y elimina. Los botones existentes permanecen disponibles.


## V2.0.5 — Slide visual
Los gestos ahora tienen animación visual: la tarjeta se desliza siguiendo el dedo, revela las acciones y completa el movimiento al modificar o eliminar. Aplicado a Notas, Listas y Pagos.


## V2.0.6 — Slide visible corregido
Gestos delegados para tarjetas creadas dinámicamente. La tarjeta ahora sigue físicamente el dedo y completa un desplazamiento visual antes de editar o eliminar.


## V2.0.7 — Swipe Directorio
Mecánica de swipe adaptada directamente de `bindSwipes()` del Directorio V2.9 para tarjetas de Notas, Listas y Pagos.


## V2.0.9 — Pagos restaurados
Se restauró el render de la pantalla de Pagos y se integró con el swipe de Directorio, sin cambiar Notas ni Listas.
