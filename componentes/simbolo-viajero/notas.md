# Símbolo viajero

**Qué es:** Un único símbolo recorre la página con el scroll, de parada en parada, y cambia de tamaño y grosor sin deformarse. Funciona en los dos sentidos.

**Proyecto de origen:** Lignum Domus (web de carpintería).

**Colores:** `#1c211e` (oscuro), `#f2f3ef` (claro), `#f99a31`, `#f99a62` y `#f2ab82` (acentos), `#5d645f` (apagado).

**Fuentes:** Fraunces (títulos) e Instrument Sans (texto), de Google Fonts.

**Cómo adaptarlo:**
- Añade paradas poniendo `data-parada` en cualquier elemento: `tal-cual`, `rodea` (con `data-k`) o `detras` (con `data-margen`). Para `detras`, el elemento necesita un `z-index` mayor que `.flyer`.
- `data-pausa` es el tiempo que se queda, en pantallas de scroll.
- Esta versión es más sencilla que la del origen: no incluye el relevo con otros marcos ni el resaltado de aros, que estaban ligados a sus secciones.
- Con movimiento reducido el símbolo se oculta: añade logos fijos si los necesitas.
- La figura de tres aros deriva del logo de Lignum Domus: para otro cliente cambia colores y proporciones, o usa otra figura.
- Los textos son de ejemplo; las fotos, si las hay, vienen de picsum.photos: sustitúyelas por las tuyas.
- Abre `index.html` en el navegador; solo necesita internet para las fuentes y las fotos.
