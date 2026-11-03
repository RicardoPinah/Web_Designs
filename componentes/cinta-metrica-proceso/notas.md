# Cinta métrica de proceso

**Qué es:** Los pasos de un proceso aparecen sobre una cinta métrica que sale de su caja con efecto de muelle y sigue al scroll en los dos sentidos. En pantallas anchas la sección queda fija y la cinta va en horizontal; en móvil y tablet baja en vertical.

**Proyecto de origen:** Lignum Domus (web de carpintería).

**Colores:** `#1c211e` (oscuro), `#f2f3ef` (claro), `#f99a31`, `#f99a62` y `#f2ab82` (acentos), `#5d645f` (apagado).

**Fuentes:** Fraunces (títulos) e Instrument Sans (texto), de Google Fonts.

**Cómo adaptarlo:**
- Cambia el color en `--acento-1` y las marcas de la regla en `background-size` de `.tape::before`.
- Si cambias el número de pasos, ajusta `repeat(7, ...)` en `.tape` y `7 * 42svh` en `.process.is-pinned`.
- El muelle se regula con `0.018` (fuerza) y `0.84` (freno) en `render`.
- La figura de tres aros deriva del logo de Lignum Domus: para otro cliente cambia colores y proporciones, o usa otra figura.
- Los textos son de ejemplo; las fotos, si las hay, vienen de picsum.photos: sustitúyelas por las tuyas.
- Abre `index.html` en el navegador; solo necesita internet para las fuentes y las fotos.
