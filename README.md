# Glass Notes V3.4 — JARVIS Notifications

Base: Glass Notes V3.3 JARVIS CORE.

## V3.4
- Añade soporte real de notificaciones del sistema mediante Service Worker.
- Panel Nexus de Notificaciones dentro de Ajustes.
- Solicitud de permiso mediante acción del usuario.
- Botón para probar una notificación.
- Avisos para pagos de hoy y pagos vencidos.
- Avisos para pendientes con fecha de hoy.
- Evita repetir el mismo aviso durante el mismo día usando localStorage.
- Los avisos abren directamente el módulo correspondiente al tocarlos.
- Service Worker incluido en el paquete y con caché versionada.
- Manifest PWA incluido.

## Importante
Esta versión habilita la capa local de notificaciones y su prueba en Android. Para recibir recordatorios programados de forma fiable cuando la PWA esté completamente cerrada, la siguiente fase debe conectar Push API + un servidor/worker de envío (VAPID); una PWA alojada únicamente en GitHub Pages no puede enviar esos pushes por sí sola.
