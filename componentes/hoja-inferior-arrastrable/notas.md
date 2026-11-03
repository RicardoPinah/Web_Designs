# Hoja inferior arrastrable

**Qué es:** Ventana que sube desde abajo y se cierra arrastrando el asa, con Escape o tocando fuera. En pantallas grandes aparece en el centro. Está hecha sin librerías.

**Proyecto de origen:** OtakuRecs (web de recomendaciones de anime y manga).

**Colores:** hoja `#FFFFFF`, contorno y asa `#1D2B53` y capa `rgba(13, 20, 40, 0.6)`. De noche, hoja `#1E2A4D`, contorno `#EAF2FF` y sombra `#FF8FAB`.

**Fuentes:** M PLUS Rounded 1c (500 y 800), desde Google Fonts.

**Cómo adaptarlo:**
- Copia las reglas de `.capa` y `.hoja`, las animaciones y las funciones `arrastrarParaCerrar` y `abrirHoja`. `.boton` y los `getElementById` son del ejemplo.
- Uso: `const { capa, cerrar } = abrirHoja(html, 'Nombre', { cerrarFuera: true })`.
- Para esperar una respuesta, escucha el evento `cerrada` de `capa`: cuenta como «Cancelar».
- Se cierra al bajar más de 100 px, o más de 30 px si es rápido. Ajusta esos números en `soltar`.
- `html` entra con `innerHTML`: escapa cualquier texto que venga de usuarios o de una API.
- No bloquea el scroll de la página ni encierra el foco de teclado dentro de la hoja. Añádelo si la ventana tiene formularios largos.
- Abre `index.html` en el navegador; solo necesita internet para la fuente.
