# CLAUDE.md · Instrucciones para Claude en Web Designs

## Qué es

La librería personal de Ricardo con diseños que se pueden volver a usar: colores y fuentes de cada proyecto (`tokens/`), piezas sueltas (`componentes/`) y secciones o páginas enteras (`paginas/`). No es una web que se publique: cada pieza es un `index.html` que se abre solo. La lista de lo que hay está en el `README.md`.

## Al empezar cada sesión

1. Este archivo ya está cargado: no lo vuelvas a leer. Del `TODO.md`, mira solo las tareas abiertas (líneas con `- [ ]`).
2. Si te dan una tarea concreta, empieza por ella.
3. Antes de tocar nada, haz `git fetch` y mira si en GitHub hay cambios que no están en local. Si los hay, di cuáles y pregunta antes de traerlos.

## Al terminar cada tarea

1. Actualiza el `TODO.md`: marca lo hecho con `(hecha día/mes/año, Nombre)` al final de la línea y añade las tareas nuevas que hayan salido, separando las de Claude y las de Ricardo.
2. Añade una entrada arriba del todo en «Registro», de una línea: fecha, qué se hizo y qué quedó a medias.
3. Haz commit en una rama de la tarea, súbela y abre un pull request. Nunca directamente a `main`.

## Cómo se añade una pieza

1. **Una carpeta** en `componentes/` (pieza suelta) o en `paginas/` (sección o página entera), con un nombre que diga qué hace y no de qué proyecto viene: `imagen-que-se-monta`, no `mueble-lignum`.
2. **`index.html` suelto:** todo dentro (estilos y script), sin depender de otros archivos de la librería. Tiene que funcionar al abrirlo. Los colores y las fuentes, copiados del archivo de `tokens/` del proyecto de origen. Si la pieza necesita un servidor para verse (por ejemplo, porque carga un modelo 3D), dilo en sus notas.
3. **`notas.md`:** qué es, proyecto de origen, colores, fuentes y cómo adaptarla. Copia la forma de las notas de otra pieza.
4. **`captura.png`:** de 1280 × 800 si es una sección; si es una pieza pequeña (un botón, una tarjeta), solo lo que ocupa.
5. **Una fila en el `README.md`**, en su tabla, con el proyecto y una frase de qué es.

Los textos son de ejemplo y las fotos, de `picsum.photos` o dibujadas en la propia página: nunca fotos, nombres ni datos reales de un cliente, y nunca claves.

## Cuándo se sube una pieza

Está pendiente de decidir por Ricardo (ver `TODO.md`). Mientras tanto: si en otro proyecto se aprueba una pieza que podría servir en otro sitio, propón subirla y espera a que diga que sí. No subas piezas por tu cuenta.

## Reglas del código

- **Sin frameworks ni compilación:** HTML, CSS y JavaScript tal cual. Las librerías de fuera, solo si la pieza no se puede hacer sin ellas (un visor de 3D), cargadas desde su dirección oficial con la versión fija, y apuntadas en las notas.
- **Comentarios en español**, cortos, que expliquen por qué.
- **Accesible:** botones de verdad, `aria-label` en los que solo llevan icono, zonas táctiles de al menos 44 px y animaciones que respetan `prefers-reduced-motion`.
- **Que funcione en el móvil**, aunque la pieza se haya pensado para escritorio.

## Comprobaciones (la misma regla en todos los proyectos)

- **Sin pedir permiso:** lo que solo devuelve texto corto, como mirar la sintaxis de un script.
- **Con permiso de Ricardo**, diciendo antes qué se quiere comprobar: abrir el navegador y hacer capturas. La `captura.png` de una pieza nueva cuenta: pide permiso antes de sacarla.
- Di siempre qué has comprobado de verdad y qué no.

## Tareas, subtareas y revisiones en el TODO.md

Hive lee así este `TODO.md`:

- **Tarea con subtareas o tarea sola:** si lo que se pide tiene varias partes que se pueden hacer y revisar por separado, apunta una tarea con el objetivo y, debajo, una subtarea por parte, con dos espacios de sangría (`  - [ ] …`). Deja en la descripción de la tarea (líneas con sangría justo debajo, antes de las subtareas) las palabras de quien lo pidió. Si es una sola cosa, una tarea sin subtareas.
- **No inventes subtareas** que nadie ha pedido: si crees que falta algo, dilo.
- **Revisiones:** lo que tiene que hacer una persona (probar, revisar, decidir, unir) va debajo de la tarea, tras una línea `  Para Ricardo:`, con la misma sangría que las subtareas. Van después de las subtareas.
- **Se marcan solas:** si una revisión se resuelve solo con unir o cerrar un pull request, termínala en `(PR 8)` (el número de ese pull request) o, si viene de un encargo de Hive, en `(encargo 13)`. Hive la marca sola cuando ese pull request se une o se cierra. Nunca en lo que haya que probar o decidir.
- **Marca en su sitio** cada subtarea y revisión hecha, con `(hecha 11/11/2026, Claude)` (la fecha de ese día). No las muevas a «Hecho» de una en una. A «Hecho» se mueve la tarea entera, con todo lo que cuelga de ella, cuando termina.
- **Un solo nivel:** no pongas subtareas dentro de subtareas.
