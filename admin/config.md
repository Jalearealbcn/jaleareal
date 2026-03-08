backend:
  name: github
  repo: Jalearealbcn/jaleareal
  branch: main
  base_url: https://auth.sveltia-cms.com
  
 
media_folder: "assets/img"
public_folder: "/assets/img"

locale: "es"

collections:
  - name: "articulos"
    label: "Artículos"
    folder: "articulos"
    create: true
    slug: "{{slug}}"
    extension: "html"
    format: "frontmatter"
    fields:
      - { label: "Título", name: "title", widget: "string" }
      - { label: "Descripción SEO", name: "description", widget: "string" }
      - { label: "Fecha", name: "date", widget: "datetime" }
      - { label: "Imagen destacada", name: "thumbnail", widget: "image", required: false }
      - { label: "Contenido", name: "body", widget: "markdown" }
