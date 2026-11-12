# Modelo 3D que gira con el scroll

**Qué es:** Una sección fija con un modelo en 3D que va girando al bajar, parada a parada, mientras se enciende el paso de texto que toca. En el móvil, o si la persona ha pedido menos animaciones, no se fija nada: el modelo se gira con el dedo y los pasos se leen seguidos.

**Proyecto de origen:** Hive (prueba piloto de 3D de la fase 3, del 12/11/2026), con los colores de Lignum Domus, que es donde más encaja: muebles reales en 3D.

**Estado:** prueba piloto. El modelo es una mesa de prueba sin texturas, hecha con un script de Blender. Falta la captura (`captura.png`) y verlo en un móvil de verdad.

**Colores:** `#1c211e`, `#2b312d` (fondo del modelo), `#f2f3ef`, `#c4c9c4` y `#f99a31` (acento).

**Fuentes:** Fraunces (títulos) e Instrument Sans (texto), de Google Fonts.

**De qué depende:**
- [`<model-viewer>`](https://modelviewer.dev) 4.0.0, de Google, cargado desde `ajax.googleapis.com` (casi 1 MB, como módulo: no frena la página).
- El modelo `mesa.glb` (13 KB) está comprimido con Draco. El visor descarga solo el descompresor de Draco desde `gstatic.com` la primera vez.
- Hace falta abrirlo desde un servidor (`http://localhost…` o la web publicada). Con doble clic en `index.html` el navegador no deja cargar el modelo.

**Cómo adaptarlo:**
- Cambia `src="mesa.glb"` por tu modelo. Para sacarlo de Blender ya comprimido: `sobremesa/blender/exportar-glb.py` del repo Hive (ver su `docs/blender-con-claude.md`).
- Los puntos de vista están en `PARADAS`: giro alrededor del modelo, altura de la cámara y distancia. Tiene que haber una parada por cada paso de texto.
- Lo que dura el recorrido es la altura de `.fijar.con-scroll` (ahora, 220 % de la pantalla además de la propia sección).
- `loading="lazy"` hace que el modelo no se descargue hasta que la sección se acerca a la pantalla. Para una web de verdad, añade `poster="imagen.webp"` con una foto del modelo: se ve al momento mientras carga.
- Los textos son de ejemplo.
