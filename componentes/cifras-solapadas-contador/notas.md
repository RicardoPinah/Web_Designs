# Cifras solapadas con contador

**Qué es:** Bloques de cifras alternando dos colores, que cuentan hasta su valor cada vez que entran en pantalla y se solapan un 30 % sobre la sección siguiente.

**Proyecto de origen:** Lignum Domus (web de carpintería).

**Colores:** `#f99a31` y `#f2ab82` para los bloques, `#1c211e` y `#f2f3ef` para los fondos.

**Fuentes:** Instrument Sans, de Google Fonts.

**Cómo adaptarlo:**
- El degradado de `.stats-band` debe usar los fondos de la sección anterior y la siguiente; el `70%` marca el solape.
- El valor va en `data-count` y también como texto, para que se vea sin JavaScript. El sufijo va fuera del `span`.
- La duración del conteo es `1600`.
- Los textos son de ejemplo; las fotos, si las hay, vienen de picsum.photos: sustitúyelas por las tuyas.
- Abre `index.html` en el navegador; solo necesita internet para las fuentes y las fotos.
