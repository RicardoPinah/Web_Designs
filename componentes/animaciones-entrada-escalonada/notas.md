# Animaciones de entrada escalonada

**Qué es:** Colección de animaciones muy cortas (0,15–0,25 s en las entradas), para que la web se sienta rápida: entrada en cascada, fundido entre páginas, rebote de contador, barra que se rellena y brillo de carga. Todas respetan «reducir movimiento».

**Proyecto de origen:** OtakuRecs (web de recomendaciones de anime y manga).

**Colores:** las animaciones no dependen de ningún color. El ejemplo usa fondo `#CFE6F7`, rosa `#FF8FAB`, rojo `#D92D20` y amarillo `#FFD23F`.

**Fuentes:** M PLUS Rounded 1c en los textos del ejemplo; las animaciones no la necesitan.

**Cómo adaptarlo:**
- Cambia `.contenedor` y `.lista-filas` por los contenedores de tu web; la cascada se aplica a sus hijos directos.
- Los retrasos son mínimos a propósito (0,02 s por elemento) y se paran en el quinto, para que una lista larga no tarde en verse.
- Pon la clase `quieto` en `<body>` al repintar una lista por un cambio pequeño, para que no parpadee.
- El fundido entre páginas solo se nota al navegar entre páginas de la misma web y en navegadores con `@view-transition`; en este ejemplo de una sola página no se ve.
- El bloque de `prefers-reduced-motion` afecta a toda la web: mantenlo siempre.
- El botón «Repetir» y las reglas bajo «Solo para el ejemplo» no hacen falta.
- Abre `index.html` en el navegador; solo necesita internet para la fuente.
