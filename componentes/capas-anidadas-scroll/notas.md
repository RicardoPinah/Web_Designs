# Capas anidadas con scroll

**Qué es:** Sección fija en la que cada marco sube dentro del anterior con su foto, mientras el texto de al lado cambia.

**Proyecto de origen:** Lignum Domus (web de carpintería).

**Colores:** `#1c211e` (oscuro), `#f2f3ef` (claro), `#f99a31`, `#f99a62` y `#f2ab82` (acentos), `#5d645f` (apagado).

**Fuentes:** Fraunces (títulos) e Instrument Sans (texto), de Google Fonts.

**Cómo adaptarlo:**
- Los tramos de scroll de cada capa están en `draw`: `(p - 0.1) / 0.36` y `(p - 0.58) / 0.36`.
- La duración total se cambia con `2 * 120svh` en `.layers.is-pinned`.
- Para otro número de capas hay que añadir su variable, sus reglas y su tramo.
- El color de separación entre aros es `--claro`: debe coincidir con el fondo de la página.
- Los textos son de ejemplo; las fotos, si las hay, vienen de picsum.photos: sustitúyelas por las tuyas.
- Abre `index.html` en el navegador; solo necesita internet para las fuentes y las fotos.
