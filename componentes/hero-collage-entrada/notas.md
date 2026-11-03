# Hero con entrada en collage

**Qué es:** Al cargar, nueve fotos entran desde fuera y forman un collage; la final queda enmarcada en aros que se abren hasta salir de la pantalla, y después llega el texto palabra a palabra.

**Proyecto de origen:** Lignum Domus (web de carpintería).

**Colores:** `#1c211e`, `#f2f3ef` y `#fff`; los aros usan `#f2ab82`, `#f99a62` y `#f99a31`.

**Fuentes:** Fraunces (títulos) e Instrument Sans (texto), de Google Fonts.

**Cómo adaptarlo:**
- Los colores de los aros van escritos en `rings` y `noRings`, dentro del script.
- `SOLO_UNA_VEZ` en el script del `head` hace que se vea solo una vez por visita. Aquí está desactivado para poder repetirla recargando.
- Si cambias el número de fotos, ajusta `layout`, `tilts` y el `9` del retraso.
- Carga nueve fotos grandes: usa versiones ligeras antes de publicar.
- Si algo falla, la entrada desaparece sola a los 12 segundos.
- Los textos son de ejemplo; las fotos, si las hay, vienen de picsum.photos: sustitúyelas por las tuyas.
- Abre `index.html` en el navegador; solo necesita internet para las fuentes y las fotos.
