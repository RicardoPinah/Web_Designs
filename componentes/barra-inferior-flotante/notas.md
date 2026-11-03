# Barra inferior flotante

**Qué es:** Barra de navegación en pastilla, separada del borde de la pantalla, con la pestaña activa en amarillo y un pequeño rebote en su icono.

**Proyecto de origen:** OtakuRecs (web de recomendaciones de anime y manga).

**Colores:** barra `#FFFFFF`, contorno y sombra `#1D2B53` y activa `#FFD23F`. De noche, barra `#1E2A4D`, contorno `#EAF2FF` y sombra `#FF8FAB`.

**Fuentes:** M PLUS Rounded 1c (800), desde Google Fonts.

**Cómo adaptarlo:**
- Para otro número de pestañas, cambia el `4` de `grid-template-columns`. Más de cinco no caben bien en el móvil.
- Deja al menos 110 px de `padding-bottom` en la página para que la barra no tape el final.
- `viewport-fit=cover` y `env(safe-area-inset-bottom)` la separan de la barra de gestos de los móviles.
- Quita el `<script>`, que solo simula el cambio de página, y pon `aria-current="page"` en el enlace de cada página.
- Los iconos son SVG de línea con trazo de 1,8 px; se pueden cambiar por otros del mismo estilo.
- Abre `index.html` en el navegador; solo necesita internet para la fuente.
