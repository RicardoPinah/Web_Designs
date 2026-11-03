# Fusión de miniaturas con scroll

**Qué es:** Al bajar del hero, las miniaturas se juntan en abanico, se funden en una y viajan hasta ocupar la foto de la sección siguiente.

**Proyecto de origen:** Lignum Domus (web de carpintería).

**Colores:** `#1c211e`, `#f2f3ef` y `#5d645f`.

**Fuentes:** Fraunces (títulos) e Instrument Sans (texto), de Google Fonts.

**Cómo adaptarlo:**
- `.merge` necesita una copia de cada miniatura, en el mismo orden, y al final la foto de destino.
- `end` en `measure` decide cuándo termina el viaje. En el origen coincidía con el inicio de una sección fija.
- Las fases están en `draw`: `gather` (se juntan) y `travel` (viajan).
- En `spin`, `2.5` es el centro del abanico para seis miniaturas: `(número - 1) / 2`.
- Los textos son de ejemplo; las fotos, si las hay, vienen de picsum.photos: sustitúyelas por las tuyas.
- Abre `index.html` en el navegador; solo necesita internet para las fuentes y las fotos.
