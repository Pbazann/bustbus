# BustBus

El juego del autobús para la previa. Se juega en un solo móvil o cada uno con el suyo, uniéndose con un código de partida.

Solo para mayores de 18 años. Bebed con cabeza: los tragos pueden ser de cualquier bebida.

## Publicar en GitHub Pages

1. Crea una cuenta en [github.com](https://github.com) (es gratis).
2. Pulsa **New repository**, ponle de nombre `bustbus`, déjalo en **Public** y pulsa **Create repository**.
3. En la página del repositorio vacío, pulsa **uploading an existing file**.
4. Arrastra **todo el contenido** de esta carpeta: `index.html`, `sw.js`, `manifest.webmanifest`, `CREDITOS.md`, `README.md` y las carpetas `cartas` e `img`. Pulsa **Commit changes**.
5. Ve a **Settings → Pages**. En **Source** elige **Deploy from a branch**, rama **main** y carpeta **/ (root)**. Pulsa **Save**.
6. En uno o dos minutos la web estará en `https://TU-USUARIO.github.io/bustbus/`.

Para actualizarla, sube de nuevo los archivos cambiados al repositorio. Los cambios aparecen en un par de minutos.

## Instalarla como app en el móvil

- **iPhone (Safari):** botón Compartir → **Añadir a pantalla de inicio**.
- **Android (Chrome):** menú ⋮ → **Instalar aplicación** o **Añadir a pantalla de inicio**.

## Cómo funciona el modo online

Cada móvil se conecta a un servidor MQTT público y gratuito (EMQX; si falla, HiveMQ). No hace falta cuenta ni servidor propio. El móvil que crea la partida hace de árbitro: guarda la baraja y decide qué pasa; los demás envían sus jugadas.

Los servidores públicos no tienen garantía de funcionamiento y cualquiera que conozca el código podría leer los nombres de la partida. Para una versión comercial conviene cambiarlos por un servicio propio (Firebase, Supabase o similar).

Ver `CREDITOS.md` para las licencias de las cartas.
