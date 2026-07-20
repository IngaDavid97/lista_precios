# Lista de precios estática

Proyecto listo para GitHub Pages. No usa base de datos, servidor, PHP, Node.js ni API propia. La web pública lee todos los productos desde productos.json.

## Actualizar precios

1. Abre actualizar.html.
2. Selecciona el archivo Excel.
3. Si abriste la herramienta directamente desde tu computadora, selecciona también el productos.json vigente. En GitHub Pages se carga solo.
4. Haz clic en Procesar Excel y revisa el resumen.
5. Descarga el nuevo productos.json.
6. Reemplaza el archivo en el repositorio.
7. Haz commit y push a GitHub. GitHub Pages publicará automáticamente la nueva lista.

La herramienta identifica las columnas por nombre sin depender de su orden: código/artículo, descripción/nombre, marca, precio IVA y precio base/valor. Si el Excel contiene solo base o solo IVA, calcula el otro precio al 15%. Los registros se comparan por código, se actualizan sin duplicados y se ordenan por marca y código.

## Uso local

Los navegadores bloquean que una página abierta con doble clic (file://) lea automáticamente productos.json. La herramienta permite seleccionar ese JSON actual. Para previsualizar index.html localmente, usa la URL de GitHub Pages o cualquier servidor estático local; no se requiere backend ni instalación en producción.
