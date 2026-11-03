# Botón que se hunde

**Qué es:** Botón amarillo con contorno y sombra dura que se hunde en su sombra al pulsarlo. Trae variantes secundaria, de peligro, pequeña y a todo el ancho.

**Proyecto de origen:** OtakuRecs (web de recomendaciones de anime y manga).

**Colores:** amarillo `#FFD23F`, tinta `#1D2B53`, peligro `#C62828` y foco rosa `#FF8FAB`. De noche, contorno `#EAF2FF` y sombra `#FF8FAB`.

**Fuentes:** M PLUS Rounded 1c (800), desde Google Fonts.

**Cómo adaptarlo:**
- El truco es que `translate(2px, 2px)` y la sombra de 3 px a 1 px compensan el mismo movimiento: si cambias uno, ajusta el otro.
- Mide 48 px de alto para que sea cómodo en el móvil; el pequeño, 40 px.
- Funciona igual en `<button>` y en `<a>`.
- El hover secundario usa `color-mix`, disponible en navegadores modernos.
- Abre `index.html` en el navegador; solo necesita internet para la fuente.
