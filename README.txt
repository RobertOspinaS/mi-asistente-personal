MI ASISTENTE PERSONAL — MVP 0.1

QUÉ INCLUYE
- Crear recordatorios con hora, categoría, notas y repetición: hoy, diario o cada 3 días.
- Marcar como hecho y eliminar tareas.
- Rutina de ejemplo editable.
- Exportar/importar copia JSON.
- Solicitud de permiso de notificaciones y prueba de notificación en 10 segundos.
- Guarda datos localmente en el navegador del dispositivo.

IMPORTANTE SOBRE LAS NOTIFICACIONES
Esta versión inicial comprueba las horas mientras la página está abierta. Los navegadores móviles pueden suspender pestañas y los temporizadores JavaScript no garantizan avisos si la página se cierra, el teléfono entra en ahorro de batería o el sistema duerme la aplicación.
Para notificaciones fiables con la aplicación cerrada hace falta una siguiente versión Android nativa con alarmas/notificaciones programadas (o un servicio específico). No confíes en esta versión para medicación crítica.

CÓMO PROBAR EN EL PC
1. Extrae el ZIP.
2. Para probar rápidamente, abre index.html en un navegador moderno. Algunas funciones, como PWA/service worker, requieren servirlo por HTTPS.
3. Para instalarlo como aplicación en Android, publica estos archivos en un sitio HTTPS (por ejemplo GitHub Pages) y abre la URL en Chrome en tu Xiaomi.
4. En Chrome Android, abre el menú ⋮ y busca “Instalar aplicación” o “Añadir a pantalla de inicio”.
5. Abre la aplicación instalada, pulsa “Activar notificaciones” y concede permiso.
6. Pulsa “Probar aviso en 10 s”. Deja la aplicación abierta y comprueba que aparece la notificación.
7. Crea un recordatorio para 2 minutos después y deja la aplicación abierta para comprobarlo.

PARA PUBLICAR CON GITHUB PAGES
1. En GitHub, crea un repositorio nuevo, por ejemplo mi-asistente-personal.
2. Sube index.html, manifest.webmanifest y sw.js a la raíz del repositorio.
3. En Settings > Pages, elige deploy desde la rama principal y la carpeta / (root).
4. Espera la URL HTTPS que te da GitHub Pages.
5. Abre esa URL en Chrome Android y sigue los pasos de instalación anteriores.

SIGUIENTE VERSIÓN RECOMENDADA
Para alertas que funcionen con la app cerrada, implementar app Android nativa (Kotlin) con AlarmManager/WorkManager, canales de notificación, acción “Hecho”, repetición configurable y persistencia. El modo de voz se puede añadir después. Los recordatorios de vitaminas deben configurarse según las indicaciones de su etiqueta o de un profesional de salud.
