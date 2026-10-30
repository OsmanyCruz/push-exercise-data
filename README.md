# push-exercise-data

Catálogo ampliado de ejercicios e imágenes para la app **push**. La app lo descarga bajo demanda (nada de esto es obligatorio para entrenar: los ejercicios base ya vienen dentro de la app).

## Estructura

- `manifest.json`: versión del catálogo, cantidad de ejercicios, cantidad de ejercicios con imágenes y peso total de las imágenes (la app lo usa para mostrar el tamaño exacto antes de "Descargar todo").
- `catalog/exercises.json`: ejercicios adicionales, en el mismo formato que `assets/data/exercise_catalog.json` de la app, más el campo `images` (rutas relativas a `images/`).
- `images/<id>/0.webp` y `1.webp`: posición inicial y final de cada ejercicio (480 px de ancho, WebP).

## Origen y licencia

Datos e imágenes derivados de [free-exercise-db](https://github.com/yuhonas/free-exercise-db) (licencia Unlicense, dominio público). Nombres, consejos y clasificación fueron traducidos y adaptados al español para push; las imágenes se redimensionaron y convirtieron a WebP.
