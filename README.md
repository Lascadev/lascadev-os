# Lascadev OS

Portafolio personal de **Luis Eduardo Ascanio Jiménez (Lascadev)**, Desarrollador Full Stack web y móvil, con estética de escritorio retro: arranque, inicio de sesión, bienvenida y un escritorio con ventanas.

## Qué incluye

- Pantalla de arranque, inicio de sesión y bienvenida
- Escritorio con ventanas que se arrastran, minimizan, maximizan y cierran
- Sobre mí (español / inglés), CV, proyectos, contacto y terminal
- Papelera con alerta de confirmación
- Freedoom jugable en una ventana (requiere teclado)

## Ejecutarlo en tu computadora

El juego carga archivos con `fetch`, así que abrir `index.html` con doble clic no basta. Usa un servidor local:

```bash
# con Python
python -m http.server 8080
# o con Node
npx serve .
```

Luego abre http://localhost:8080

## Publicarlo con GitHub Pages

1. Sube el contenido de esta carpeta a un repositorio.
2. En el repositorio: **Settings → Pages → Build and deployment**, elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
3. En uno o dos minutos queda en `https://<tu-usuario>.github.io/<nombre-del-repo>/`.

Si nombras el repositorio `<tu-usuario>.github.io`, la dirección será directamente `https://<tu-usuario>.github.io/`.

## Estructura

```
index.html                  Portafolio completo (HTML, CSS y JS en un archivo)
freedoom/game.html          Página del juego que se carga dentro de la ventana
freedoom/websockets-doom.*  Motor del juego compilado a WebAssembly
freedoom/freedoom1.b64.txt  Datos del juego (Freedoom Phase 1, gzip + base64)
freedoom/default.cfg.txt    Configuración de controles
freedoom/COPYING.txt        Licencia de Freedoom
```

## Licencias de terceros

- **Freedoom**: licencia BSD modificada, ver `freedoom/COPYING.txt`. https://freedoom.github.io/
- **Motor doom-wasm** (basado en Chocolate Doom): GPL-2.0. Código fuente: https://github.com/cloudflare/doom-wasm

El logo, el fondo, los íconos y el sonido de inicio de Lascadev OS son originales. El estilo visual está inspirado en los escritorios de principios de los 2000; no incluye logos, fondos ni sonidos de Microsoft.
