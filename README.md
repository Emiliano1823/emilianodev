
raw
Readme · MD
# Emiliano López — Portafolio Personal
 
Portafolio web personal. Ultra minimalista, tipografía editorial, dark/light mode. Un solo archivo `index.html` — sin frameworks, sin dependencias, sin npm.
 
---
 
## Vista previa
 
| Light mode | Dark mode |
|---|---|
| Fondo blanco `#ffffff`, textos negros `#0f0f0f` | Fondo negro `#0f0f0f`, textos blancos `#f0f0f0` |
 
---
 
## Stack
 
| Tecnología | Uso |
|---|---|
| **HTML5** | Estructura semántica |
| **CSS3** | Variables, Grid, animaciones, dark/light mode |
| **JavaScript (ES6)** | IntersectionObserver, toggle de tema, menú móvil |
| **Instrument Serif** | Tipografía de títulos (Google Fonts) |
| **Inter** | Tipografía de cuerpo (Google Fonts) |
| **JetBrains Mono** | Labels técnicos y tags (Google Fonts) |
 
> Las fuentes se cargan desde Google Fonts. Se requiere conexión a internet para verlas.
 
---
 
## Estructura
 
```
portafolio/
└── index.html   ← Todo el proyecto en un solo archivo
```
 
CSS y JS están embebidos directamente en el HTML para máxima portabilidad y velocidad de carga. Si el proyecto crece, se puede separar en:
 
```
portafolio/
├── index.html
├── style.css
└── main.js
```
 
---
 
## Secciones
 
| # | Sección | Descripción |
|---|---|---|
| 01 | **Hero** | Nombre, rol animado, badge disponible, métricas rápidas |
| 02 | **Sobre mí** | Texto descriptivo, stats y soft skills |
| 03 | **Skills** | Tabla por categoría: lenguajes, frontend, backend, DB, herramientas |
| 04 | **Proyectos** | Lista editorial con stack por proyecto |
| 05 | **Experiencia** | Rancho El Mogote con indicador "en curso" |
| 06 | **Educación** | Títulos académicos y certificaciones |
| 07 | **Contacto** | Email, teléfono, ubicación |
 
---
 
## Características
 
- **Dark / Light mode** con toggle en la nav — preferencia guardada en `localStorage`
- **Responsive** — adaptado para móvil, tablet y escritorio
- **Scroll reveal** — elementos aparecen al entrar en pantalla con `IntersectionObserver`
- **Rol animado** — el subtítulo del hero rota cada 4 segundos con fade
- **Cero dependencias** — no requiere npm, bundler ni servidor
- **Sin imágenes externas** — íconos SVG inline, sin librerías de íconos
---
 
## Ejecutar localmente
 
### Opción 1 — Live Server (recomendada)
 
1. Instala [VS Code](https://code.visualstudio.com/)
2. Instala la extensión **Live Server** de Ritwick Dey
3. Abre `index.html` en VS Code
4. Clic en **Go Live** (barra inferior derecha)
5. Se abre en `http://127.0.0.1:5500` con recarga automática
### Opción 2 — Directo en el navegador
 
```bash
git clone https://github.com/tu-usuario/portafolio.git
cd portafolio
 
# Windows
start index.html
 
# macOS
open index.html
 
# Linux
xdg-open index.html
```
 
---
 
## Publicar en GitHub Pages
 
1. Sube el repositorio a GitHub
2. **Settings → Pages → Branch:** `main` / `/ (root)` → **Save**
3. En unos minutos disponible en `https://tu-usuario.github.io/portafolio/`
También funciona con **Netlify** y **Vercel** con drag & drop del archivo `index.html`.
 
---
 
## Conceptos del código
 
| Concepto | Dónde |
|---|---|
| `CSS Custom Properties` | `:root` y `[data-theme="dark"]` para los dos temas |
| `data-theme` attribute | Toggle en `<html>` que activa el modo oscuro |
| `localStorage` | Guarda la preferencia de tema entre visitas |
| `IntersectionObserver` | Activa `.in` cuando `.r` entra al viewport |
| `transition` en `body` | Cambio suave de colores al alternar el tema |
| `CSS Grid` | Layout de secciones y tabla de skills |
| `clamp()` | Tipografía fluida que escala con el viewport |
| SVG inline | Íconos sin dependencias externas |
 
---
 
## Autor
 
**Jesús Emiliano López Espinoza**
Ingeniero en Sistemas Computacionales — TecNM La Piedad
 
- emiliano.espinoza118@gmail.com
- 352 132 1113
- La Piedad, Michoacán, México
---
 
*© 2026 Jesús Emiliano López Espinoza*
 
