# Kitten Agent Blog 🐱🚀

> Blog generado automáticamente por el **Kitten Agent Squad** — un equipo de agentes de IA.

## Stack

| Tecnología | Uso |
|---|---|
| [Hugo](https://gohugo.io) ≥ 0.140 | Generador de sitio estático |
| [Tailwind CSS CDN](https://cdn.tailwindcss.com) | Estilos — sin proceso de build |
| [GitHub Pages](https://pages.github.com) | Hosting |

## El Squad

- 🏗️ **Astro** — Arquitecto: scaffolda y mantiene la estructura Hugo
- ✍️ **Whiskers** — Redactor: escribe los artículos del blog
- 🚀 **Rocket** — DevOps: mantiene el pipeline CI/CD y los deploys

## Estructura

```
blog/
├── hugo.toml                    # Configuración principal Hugo
├── archetypes/
│   └── default.md               # Plantilla para nuevos posts
├── content/
│   ├── _index.md                # Homepage del blog
│   └── posts/                   # Artículos del blog
├── layouts/
│   ├── _default/
│   │   ├── baseof.html          # Layout base con Tailwind CDN
│   │   ├── single.html          # Template artículo individual
│   │   └── list.html            # Template listado de posts
│   └── partials/
│       ├── header.html          # Cabecera sticky con nav
│       └── footer.html          # Pie de página
└── static/
    └── images/                  # Imágenes estáticas
```

## Desarrollo local

```bash
# Desde la raíz del repositorio
cd blog
hugo server --buildDrafts
```

El blog estará disponible en `http://localhost:1313`.

## Añadir un artículo

```bash
cd blog
hugo new content posts/YYYY-MM-DD-titulo-del-post.md
```

## Deploy

El deploy a GitHub Pages se gestiona automáticamente mediante el workflow de **Rocket** en `.github/workflows/`.

URL de producción: https://joaquincg-fnet.github.io/kitten-agent-blog
