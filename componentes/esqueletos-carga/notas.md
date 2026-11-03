# Esqueletos de carga

**Qué es:** Huecos grises que laten suavemente con la forma de lo que va a salir (filas, personas o portadas), en vez de un «Cargando…».

**Proyecto de origen:** OtakuRecs (web de recomendaciones de anime y manga).

**Colores:** huecos `#A9C6DE` sobre fondo `#CFE6F7`. De noche, `#33416A` sobre `#121A33`.

**Fuentes:** M PLUS Rounded 1c en los textos del ejemplo; los huecos no la necesitan.

**Cómo adaptarlo:**
- Copia las reglas `.esqueleto-*`, `.oculto-visual`, `@keyframes latir` y la función `esqueletoHTML`. El resto es del ejemplo.
- Uso: `lista.innerHTML = esqueletoHTML('fila', 3)` y sustitúyelo cuando lleguen los datos. En un `<ul>`, pasa `'li'` como tercer argumento.
- Los huecos deben medir lo mismo que el contenido real, para que la página no salte: ajusta los tamaños de `.esqueleto-bloque`.
- Quien usa lector de pantalla oye «Cargando…» gracias al texto oculto.
- El tipo `persona` estaba en OtakuRecs solo como clase de CSS; aquí también lo admite la función.
- Abre `index.html` en el navegador; solo necesita internet para la fuente.
