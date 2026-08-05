# María José | Carta digital Makeup & Beauty

Catálogo móvil: presentación, portafolios por servicio y WhatsApp.

## Enlace público (para clientes)

**Comparte este enlace** (no muestra tu usuario de GitHub):

**https://majo-makeup-ec.vercel.app**

Alternativa (incluye tu usuario de GitHub en la URL):  
https://jeansitogoat.github.io/mj-makeup-carta/

Repositorio (privado o solo para ti): [github.com/Jeansitogoat/mj-makeup-carta](https://github.com/Jeansitogoat/mj-makeup-carta)

### Dominio propio (opcional, más profesional)

En Vercel → proyecto **majo-makeup-ec** → Settings → Domains puedes añadir por ejemplo `carta.tudominio.com` y el link deja de decir `vercel.app`.

## Importante: cómo compartir con clientes

**No envíes solo el archivo `.html` por WhatsApp.** En iPhone y Android se ve roto (sin diseño, sin fotos, sin video) porque:

1. El HTML necesita la carpeta **`media/`** (fotos y video) en la misma ruta.
2. El diseño usa **internet** (Tailwind, fuentes e iconos desde CDN). Al abrir un archivo suelto, muchos móviles bloquean eso.
3. Lo correcto es compartir un **enlace web** `https://...` en bio de Instagram, historias o WhatsApp.

### Opción recomendada: publicar en internet (gratis)

**Vercel o Netlify** (rápido, enlace tipo `https://majo-makeup.vercel.app`):

1. Sube el proyecto a **GitHub** (repositorio con `index.html` + carpeta `media/`).
2. Entra en [vercel.com](https://vercel.com) → Import Project → elige el repo → Deploy.
3. Comparte la URL que te den.

**GitHub Pages** (también gratis):

1. Repo en GitHub con rama `main`.
2. Settings → Pages → Source: Deploy from branch → `/ (root)`.
3. Enlace: `https://tu-usuario.github.io/nombre-repo/`

Git sirve para **guardar el proyecto y desplegar**; los clientes finales no necesitan Git, solo el **link**.

### Probar bien en el celular (antes de publicar)

En la misma Wi‑Fi del PC:

```bash
npm run dev
```

Abre en el teléfono: `http://IP-DE-TU-PC:3000` (no abras el HTML desde Archivos).

### Estructura del proyecto

```
MJ-makeup-carta/
├── index.html          ← página principal (hosting)
├── mj_makeup_html.html ← copia del mismo contenido (opcional)
├── media/              ← obligatorio (no borrar)
│   ├── hero-inicio.png
│   ├── novia.mp4
│   └── ...
└── package.json
```

## Personalizar

- WhatsApp: variable `telefonoMajo` en el script del HTML.
- Instagram: enlace a [@majo_makeup.ec](https://www.instagram.com/majo_makeup.ec/).
- Fotos/video: reemplazar archivos en `media/` (mismos nombres) o editar rutas en `portafolios` dentro del script.
