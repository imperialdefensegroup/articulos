PASOS PARA ARREGLAR "Dirección de sitemap no válida" EN SEARCH CONSOLE

1) Asegúrate de estar en la propiedad correcta en Search Console:
   - Tipo de propiedad: URL prefix
   - URL EXACTA: https://imperialdefensegroup.github.io/articulos/
   (Si la propiedad es otra, Google puede decir que la dirección del sitemap es inválida.)

2) Sube estos archivos a la raíz del repo imperialdefensegroup/articulos:
   - _config.yml (este que incluyo)
   - robots.txt (este que incluyo)
   (Si ya los tienes, sustituye o fusiona su contenido con lo de este paquete.)

3) Haz un commit para forzar la reconstrucción de GitHub Pages.

4) Verifica en el navegador que existe el sitemap:
   https://imperialdefensegroup.github.io/articulos/sitemap.xml
   - Si devuelve XML, perfecto.
   - Si 404, revisa que en _config.yml estén:
       url: "https://imperialdefensegroup.github.io"
       baseurl: "/articulos"
     y que el plugin jekyll-sitemap esté en "plugins".

5) En Search Console, dentro de la propiedad https://imperialdefensegroup.github.io/articulos/,
   ve a Sitemaps y envía:
   - O BIEN: sitemap.xml
   - O BIEN: https://imperialdefensegroup.github.io/articulos/sitemap.xml

6) Si sigue fallando:
   - Asegúrate de que GitHub Pages esté activo (Settings → Pages → Branch: main / root).
   - Vacía caché o intenta en modo incógnito.
   - Comprueba que robots.txt NO bloquea (este archivo permite todo).
