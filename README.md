# 🎵 Cultura Musical

Experiencia web interactiva sobre la cultura musical a través de los años: desde los primeros instrumentos de la prehistoria hasta la era del streaming, con línea del tiempo por épocas, las ramas (subgéneros) de cada género musical, un estudio de ritmos y un quiz.

**🌐 Ver en vivo:** https://withergamer36.github.io/cultura-musical/

## Características

- **🎛️ Estudio de ritmos** — secuenciador de 16 pasos con síntesis en tiempo real (Web Audio API): bombo, caja, hi-hat y bajo, 7 presets de género (rock, metal, punk, hip-hop, reggaetón, house, techno), tempo ajustable, edición de patrones y visualizador de espectro.
- **🧠 Quiz interactivo** — 10 preguntas con explicación en cada respuesta, orden aleatorio, mejor marca guardada en el dispositivo y compartir resultado.
- **🔍 Buscador global** (`Ctrl+K`) — encuentra cualquier época, género o subgénero con navegación por teclado y salto directo a la sección.
- **📖 Fichas de subgéneros** — cada chip abre un modal con descripción, enlace a Wikipedia y botón para oír el ritmo de su familia.
- **⭐ Favoritos** — marca tus géneros favoritos (persisten en el dispositivo) y fíltralos.
- **🌙/☀️ Tema oscuro y claro** con memoria de preferencia (atajo: `T`).
- **📶 PWA instalable** — funciona sin conexión gracias a un service worker (`sw.js` + `manifest.webmanifest`).
- **✨ Detalles de producto** — barra de progreso de lectura, animaciones al hacer scroll, botón "volver arriba", toasts, compartir nativo, SEO completo (Open Graph, Twitter Cards, JSON-LD) y diseño responsive.
- Página 100 % estática (`index.html`) — sin dependencias ni proceso de build; todo el audio se sintetiza en el navegador, sin archivos de sonido.

## Contenido

- Línea del tiempo: de la prehistoria (40.000 a.C.) a la era del streaming
- 13 familias de géneros con más de 110 subgéneros

## Desarrollo

No hay build: abre `index.html` con cualquier servidor estático (el service worker requiere `http://localhost` o `https`). Por ejemplo:

```bash
npx serve .
```
