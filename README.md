# JIKU SOLUTIONS — Página web

Réplica de la página de JIKU SOLUTIONS (`jikusolutions.base44.app`), construida
como un solo archivo HTML sin dependencias de Base44, lista para publicarse en
GitHub Pages y fácil de modificar.

## Estructura

| Archivo | Descripción |
|---|---|
| `index.html` | Toda la web: estilos, contenido y scripts en un solo archivo. |
| `assets/logo.png` | Logo de JIKU SOLUTIONS. |
| `.github/workflows/deploy.yml` | Despliegue automático a GitHub Pages en cada push. |

## Cómo modificar la web

### Opción 1 — Modo edición visual (sin tocar código)

1. Abre la página añadiendo `?editar` al final de la dirección
   (por ejemplo `https://tu-usuario.github.io/Jiku-Webpage/?editar`
   o `index.html?editar` si la abres en tu computadora).
2. Haz clic sobre cualquier texto (títulos, párrafos, botones, teléfono,
   correo…) y escríbelo de nuevo. Los cambios se guardan automáticamente
   en tu navegador.
3. Cuando termines, pulsa **Descargar HTML** en la barra inferior: obtendrás
   un `index.html` con tus cambios ya aplicados.
4. Sube ese archivo al repositorio (reemplazando el `index.html` actual) y
   GitHub Pages publicará la nueva versión automáticamente.

Botones de la barra de edición:

- **Descargar HTML**: genera el archivo con tus cambios listos para subir.
- **Restablecer**: borra tus cambios y vuelve a los textos originales.
- **Salir**: cierra el modo edición (tus cambios quedan guardados en el navegador).

### Opción 2 — Editar el código directamente

Todo está en `index.html`, organizado con comentarios en español:

- **Colores**: al inicio del `<style>`, en el bloque `:root` (variables como
  `--azul`, `--morado`, `--fondo`…). Cambia un valor y toda la web se actualiza.
- **Textos**: busca la sección correspondiente (`HERO`, `SERVICIOS`,
  `POR QUÉ JIKU`, `CTA`, `PIE DE PÁGINA`) y edita el texto dentro de las
  etiquetas HTML.
- **Fuente**: se usa [Sora](https://fonts.google.com/specimen/Sora) de Google
  Fonts; puedes cambiarla en el `<link>` de fuentes y en la variable `--fuente`.
- **Logo**: reemplaza `assets/logo.png` por tu propia imagen (idealmente cuadrada).

## Ver la web en tu computadora

No necesita instalación: abre `index.html` con doble clic, o si prefieres un
servidor local:

```bash
python3 -m http.server 8000
# y visita http://localhost:8000
```
