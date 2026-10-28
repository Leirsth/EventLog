EVENTLOG — PROTOTIPO PWA

Contenido:
- index.html: interfaz y lógica de EventLog
- manifest.webmanifest: metadatos para instalar en la pantalla de inicio
- sw.js: caché offline
- icon.svg: icono de la aplicación

IMPORTANTE SOBRE PRIVACIDAD
El sitio estático solo entrega el código de la aplicación. Los registros se guardan en localStorage del navegador/dispositivo y no se envían a un servidor mediante el código de esta app. No publiques tu CSV de TapDiary ni una versión del HTML que lleve tus registros precargados.

CÓMO PUBLICAR GRATIS CON GITHUB PAGES (desde Safari)
1. Inicia sesión o crea una cuenta en GitHub.
2. Crea un repositorio nuevo llamado eventlog (puede ser público; contiene solo el código, no tus datos).
3. Usa Add file > Upload files y sube index.html, manifest.webmanifest, sw.js e icon.svg desde esta carpeta descomprimida.
4. En Settings > Pages, elige Deploy from a branch, selecciona main y /(root), y guarda.
5. Espera a que GitHub Pages muestre la URL HTTPS del sitio.
6. Abre esa URL en Safari. Importa tu CSV desde el selector de archivos.
7. Para instalar: botón Compartir de Safari > Añadir a pantalla de inicio.
8. Abre la app una vez con conexión y luego activa modo avión para probar el funcionamiento offline.

LIMITACIONES
- Es un prototipo. localStorage puede borrarse si se eliminan los datos del sitio; usa Exportar CSV y Copia JSON regularmente.
- La instalación offline requiere abrir la versión HTTPS al menos una vez para que el service worker almacene los archivos.
- El prototipo todavía no se integra automáticamente con Atajos de Apple.
- El CSV de TapDiary debe seleccionarse manualmente desde Importar CSV.
