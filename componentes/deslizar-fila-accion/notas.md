# Deslizar una fila para hacer una acción

**Qué es:** Gesto de deslizar una fila a la derecha. Al lado aparece una franja con lo que va a pasar, que se vuelve amarilla al pasar el punto en que se hace. Está hecho sin librerías.

**Proyecto de origen:** OtakuRecs (web de recomendaciones de anime y manga).

**Colores:** franja `#FFFFFF`, amarillo `#FFD23F` al llegar al punto y contorno `#1D2B53`. De noche, franja `#1E2A4D` y contorno `#EAF2FF`.

**Fuentes:** M PLUS Rounded 1c (500 y 800), desde Google Fonts.

**Cómo adaptarlo:**
- Pon `data-deslizar="id"` en cada fila y llama a `activarDeslizar(contenedor, { texto, alDeslizar })`.
- `alDeslizar` recibe el id y la fila. El punto de la acción está en `UMBRAL_DESLIZAR` y el recorrido máximo es de 150 px.
- Deja `conRaton: true` solo para probarlo en el ordenador. En OtakuRecs era solo táctil, para no chocar con los clics y la selección de texto.
- El contenedor recorta lo que sobresale: deja un poco de `padding` a la derecha y abajo si las filas tienen sombra.
- Úsalo solo en listas de filas, no en rejillas ni en filas que ya se deslizan en horizontal.
- Todo lo que se haga con el gesto debería tener también un botón, porque no es fácil de descubrir.
- Cambios respecto al original: la opción `conRaton`, la captura del puntero y que cancelar el gesto no haga la acción.
- Abre `index.html` en el navegador; solo necesita internet para la fuente.
