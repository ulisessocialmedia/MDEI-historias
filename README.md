# Historias MDEI

Generador de historias de Instagram para los doctores de la red MDEI.
Los doctores solo aportan la idea: el diseño, el logo, los colores y las
tipografías están fijados.

## Contenido

| Archivo | Para qué |
|---|---|
| `index.html` | La aplicación completa. Un solo archivo, con el logo incrustado. |
| `manifest.webmanifest` | Permite instalarla en el móvil ("Añadir a pantalla de inicio"). |
| `favicon.ico`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | Iconos. |
| `.nojekyll` | Evita que GitHub Pages procese los archivos. No borrar. |

## Publicarla con GitHub Pages

1. Entra en https://github.com y crea un repositorio nuevo: botón **New**.
   Nombre, por ejemplo, `historias-mdei`. Marca **Public** (Pages es gratis
   solo en repos públicos del plan Free). No añadas README.
2. En el repo vacío pulsa **uploading an existing file**.
3. Arrastra **el contenido de esta carpeta**, no la carpeta en sí: tienen
   que quedar `index.html` y los demás archivos en la raíz del repositorio.
   Si `.nojekyll` no aparece al arrastrar, actívalo en Finder con
   `Cmd + Shift + .` para ver los archivos ocultos.
4. Pulsa **Commit changes**.
5. Ve a **Settings → Pages**. En *Source* elige **Deploy from a branch**,
   rama `main` y carpeta `/ (root)`. Guarda.
6. Espera uno o dos minutos y recarga esa misma pantalla: aparece la URL,
   del tipo `https://TUUSUARIO.github.io/historias-mdei/`. Esa es la que
   mandas a los doctores.

Para actualizarla más adelante: sube el nuevo `index.html` al repositorio
(**Add file → Upload files**, mismo nombre) y confirma el reemplazo. La URL
no cambia.

## Dominio propio (opcional)

En **Settings → Pages → Custom domain** escribe, por ejemplo,
`historias.mdei.institute`, y en tu proveedor de DNS crea un registro CNAME
de `historias` apuntando a `TUUSUARIO.github.io`. Marca luego
*Enforce HTTPS*.

## Notas

- Requiere conexión a internet para cargar las tipografías DM Sans y
  Manrope desde Google Fonts. Todo lo demás funciona sin conexión.
- Las fotos que suben los doctores no salen de su dispositivo: la imagen se
  compone en el navegador y se descarga desde ahí. No hay servidor.
- Esta versión no guarda historial compartido entre doctores. Esa función
  solo existe en la versión alojada en Claude.
- `noindex` impide que Google la indexe, pero la página es pública para
  quien tenga el enlace.
