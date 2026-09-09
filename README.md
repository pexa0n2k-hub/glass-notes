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


## V2.1.0 — Pagos restaurados de base estable
Se recuperó el renderizador completo de Pagos desde la versión estable V2.0.2, manteniendo el resto de la interfaz y los gestos de V2.0.9.


## V2.1.1 — Pagos Pro
Pagos usa un gesto independiente por tarjeta para no bloquear sus botones internos. El arrastre horizontal sigue la tarjeta, muestra Modificar/Eliminar y completa la animación antes de ejecutar la acción.


## V2.1.2 — Pagos funcionando
Se reincorporó el renderizador completo de Pagos desde la base estable V2.0.2. La navegación a Pagos queda explícita y el módulo vuelve a mostrar movimientos, crear, editar, marcar pagado y eliminar.


## V2.1.4 — Swipe Pagos estable
Pagos usa exactamente la estructura swipe-wrap/swipe-card del sistema que ya anima Notas y Listas. Se elimina el listener global duplicado.

## V2.1.5 — Respaldo dentro de Ajustes

- El respaldo y la restauración se mantienen exclusivamente dentro de **Ajustes**.
- No se inyecta ningún panel de respaldo en `document.body`.
- No se modifica la lógica de Notas, Pendientes ni Pagos.
- Se actualiza el nombre de caché del Service Worker para GitHub Pages.


## V2.2.0 — Buscador Global
Búsqueda de solo lectura en Notas, Listas y Pagos.


## V2.2.1 — Resultados inteligentes
Los resultados del buscador ahora pueden abrir el elemento correspondiente.
