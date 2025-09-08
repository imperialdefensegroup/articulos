Guía rápida — Verificación de propiedad (Search Console)

1) Sube el archivo 'google3969f57c69dd6c78.html' a la **raíz** del repo:
   imperialdefensegroup/articulos
   (junto a _config.yml, index.md, robots.txt, etc.)

   Estructura ejemplo:
   articulos/
    ├─ _config.yml
    ├─ index.md
    ├─ robots.txt
    ├─ _posts/
    └─ google3969f57c69dd6c78.html  👈 aquí

2) Haz Commit y espera a que GitHub Pages regenere el sitio.

3) Comprueba en el navegador que la URL carga el archivo (texto plano):
   https://imperialdefensegroup.github.io/articulos/google3969f57c69dd6c78.html

4) Ve a Google Search Console, selecciona la propiedad
   https://imperialdefensegroup.github.io/articulos/
   y pulsa **Verificar**.

Notas:
- No cambies el **nombre** ni el **contenido** del archivo.
- Si prefieres verificación por meta tag, pega en _config.yml:
  google_site_verification: "google3969f57c69dd6c78.html"
  (con jekyll-seo-tag se insertará en <head> automáticamente).
