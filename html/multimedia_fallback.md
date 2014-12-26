##Multimedia Fallback
Para los elementos multimedia tal como las imágenes, videos u objetos animados por canvas. Asegurate de ofrecer un elemento alternativo. Para el caso de las imagenes por ejemplo, esto implica agregar un texto alternativo muy descriptivo. Para los videos o audios esto implica poner recursos alternativos y una descripcion dentro del elemento en caso que no soporte dicho elemento.

Si las imagenes son puramente decorativa se recomienda insertarlas por estilos css en vez de usar la etiqueta img.
>**Ejemplo:**
>```html
<!-- No recomendado -->
<img src="producto.png">
<!-- Recomendado -->
<img src="producto.png" alt="Producto de la emrpesa.">
```
