# Fondo de cielo con nubes y estrellas

**Qué es:** Fondo que se repite, hecho con un SVG dentro del CSS: nubes de día y estrellas de noche, sin archivos de imagen.

**Proyecto de origen:** OtakuRecs (web de recomendaciones de anime y manga).

**Colores:** `#CFE6F7` (claro), `#8FB3D1` (intermedio) y `#121A33` (oscuro). Nubes blancas o `#E4EEF7`, estrellas `#EAF2FF`.

**Fuentes:** M PLUS Rounded 1c solo en el texto de ejemplo; el fondo no la necesita.

**Cómo adaptarlo:**
- Copia las variables `--fondo` y `--cielo` de cada tema y las tres reglas de `background`.
- `background-size` debe coincidir con el `width` y `height` del SVG (420 × 340).
- Para cambiar la intensidad, edita `fill-opacity` dentro del SVG; para el color, `fill` (el `#` se escribe `%23`).
- Sin `data-tema` en `<html>` sigue el modo del sistema; los botones solo están para probarlo.
- Abre `index.html` en el navegador; solo necesita internet para la fuente.
