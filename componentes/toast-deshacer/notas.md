# Aviso con Deshacer

**Qué es:** Aviso flotante que entra desde abajo y desaparece solo. Con la opción `deshacer` lleva un botón y dura 5,5 s en vez de 3,2 s.

**Proyecto de origen:** OtakuRecs (web de recomendaciones de anime y manga).

**Colores:** usa los colores invertidos, tinta `#1D2B53` de fondo y blanco de texto, con sombra y subrayado `#FF8FAB`. De noche, fondo `#EAF2FF` y texto `#1E2A4D`.

**Fuentes:** M PLUS Rounded 1c (800), desde Google Fonts.

**Cómo adaptarlo:**
- Copia `.toast`, `.toast-deshacer`, la animación y la función `toast`. `.boton` y el contador son del ejemplo.
- Uso: `toast('Guardado')` o `toast('Añadido', { deshacer: async () => { … } })`.
- `deshacer` puede ser asíncrona: si falla, sale «No se pudo deshacer.».
- Si la página tiene barra inferior, sube el `bottom`: en OtakuRecs eran 92 px.
- Con una ventana abierta conviene sacarlo arriba: `body:has(.capa) .toast { top: 16px; bottom: auto; }`.
- El texto entra con `textContent`, así que no hace falta escaparlo.
- Abre `index.html` en el navegador; solo necesita internet para la fuente.
