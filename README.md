# Sitio de la clase · Computación

Sitio estático (HTML y CSS, sin instalar nada). Estructura:

- `index.html` — inicio con los grupos
- `prepa/index.html` — Cultura digital, 1.º de preparatoria
- `assets/estilos.css` — estilos de todo el sitio
- `descargas/` — archivos que los alumnos descargan

## Publicar en Vercel (sin programar)

1. Entra a vercel.com e inicia sesión (puede ser con tu cuenta de Google o GitHub).
2. **Opción fácil:** crea un repositorio en GitHub, sube esta carpeta (botón "Add file › Upload files") y en Vercel elige **Add New › Project › Import** ese repositorio.
3. En la configuración deja **Framework Preset: Other** y no cambies nada más. Pulsa **Deploy**.
4. Vercel te da una dirección tipo `tu-proyecto.vercel.app`. Ya funciona.

Cada vez que cambies un archivo en GitHub, Vercel actualiza el sitio solo.

## Conectar tu dominio (después)

1. En Vercel: proyecto › **Settings › Domains** › escribe tu dominio (por ejemplo `clases.tudominio.com`).
2. Vercel te dice qué registro agregar. Lo usual:
   - Subdominio (`clases.tudominio.com`): registro **CNAME** con nombre `clases` y valor `cname.vercel-dns.com`.
   - Dominio principal (`tudominio.com`): registro **A** con valor `76.76.21.21`.
3. Esos registros se agregan donde administras el dominio. Los dominios de Google Domains pasaron a **Squarespace**: entra a Squarespace › Domains › DNS settings.
4. Puede tardar desde minutos hasta unas horas. Usa siempre el valor exacto que muestre Vercel.

## Cómo actualizar contenido

- Fechas: busca la sección `id="fechas"` en `prepa/index.html`.
- Agregar una descarga: copia el archivo a `descargas/` y duplica una tarjeta en la sección `id="descargas"`.
