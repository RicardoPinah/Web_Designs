# Portada con etiqueta de formato

**Qué es:** Portada 5:7 con contorno y etiqueta arriba a la izquierda. La imagen entra con un fundido y se acerca al pasar por encima; sin imagen, queda un color. Trae rejilla y tres tamaños fijos.

**Proyecto de origen:** OtakuRecs (web de recomendaciones de anime y manga).

**Colores:** contorno y etiqueta `#1D2B53`, color sin imagen `#FF8FAB` y título al pasar por encima `#C2185B`. De noche, contorno y etiqueta `#EAF2FF`, y título `#FF8FAB`.

**Fuentes:** M PLUS Rounded 1c (800), desde Google Fonts.

**Cómo adaptarlo:**
- Pon el color propio de cada elemento con `style="background-color: …"`: se ve mientras carga la imagen y evita huecos vacíos.
- Las medidas fijas y `aspect-ratio` reservan el sitio, así que la página no salta al cargar.
- La etiqueta sirve para cualquier categoría: formato, género, «Nuevo»…
- `alt=""` es correcto si el título va al lado; si la portada va sola, pon un texto alternativo.
- Las fotos vienen de picsum.photos y los textos son de ejemplo: sustitúyelos por los tuyos.
- Abre `index.html` en el navegador; necesita internet para la fuente y las fotos.
