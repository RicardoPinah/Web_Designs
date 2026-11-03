# Tarjeta con sombra dura

**Qué es:** Tarjeta de dibujo animado con contorno de 2 px y sombra dura sin difuminar. Si es un enlace, se levanta al pasar por encima.

**Proyecto de origen:** OtakuRecs (web de recomendaciones de anime y manga).

**Colores:** contorno y sombra `#1D2B53`, fondo de tarjeta `#FFFFFF`. De noche, contorno `#EAF2FF`, sombra `#FF8FAB` y fondo `#1E2A4D`.

**Fuentes:** M PLUS Rounded 1c (500 y 800), desde Google Fonts.

**Cómo adaptarlo:**
- Copia `.tarjeta` y `a.tarjeta:hover`, con las variables de `:root`.
- El carácter lo dan `--grosor`, `--radio` y el desplazamiento de `box-shadow`: mantén la sombra sin difuminar.
- De noche conviene un color de sombra llamativo; una sombra oscura no se vería sobre el fondo.
- Los textos son de ejemplo.
- Abre `index.html` en el navegador; solo necesita internet para la fuente.
