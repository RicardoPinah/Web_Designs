# Hero con miniaturas

**Qué es:** Hero a pantalla completa con miniaturas seleccionables, cambio automático cada 6 segundos, zoom lento y barra de progreso. Se pausa al pasar el ratón o al enfocar las miniaturas.

**Proyecto de origen:** Lignum Domus (web de carpintería).

**Colores:** `#1c211e`, `#f99a31` y `#fff`.

**Fuentes:** Fraunces (títulos) e Instrument Sans (texto), de Google Fonts.

**Cómo adaptarlo:**
- Cada foto necesita su `.slide` y su `.thumb`, en el mismo orden.
- Para cambiar el tiempo, modifica a la vez `6000` en `play`, `6s` en `drift` y `6s` en `thumb-progress`.
- Las miniaturas usan aquí la foto grande: en producción, usa una versión pequeña.
- Los textos son de ejemplo; las fotos, si las hay, vienen de picsum.photos: sustitúyelas por las tuyas.
- Abre `index.html` en el navegador; solo necesita internet para las fuentes y las fotos.
