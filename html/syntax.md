Syntax
-------------

- Se tiene que usar dos espacios para tu indentado de código
- Se tiene que usar doble comilla ( " " ) para declarar a tus atributos, nunca uses comilla simple ( ' ' )
- No incluyas las barras de cierre en los elementos como input, br, img, hr
```html 
<!-- Malo -->
<input/> <br/> <img/> <hr/>
<!-- Bueno -->
<input> <br> <img> <hr> 
```
- No omitir las etiquetas de cierre
```html
<!-- Malo -->
<li> <html> <body>
<!-- Bueno -->
<li></li> <html></html> <body></body>
```
Ejemplo General
```html
<!DOCTYPE html>
<html>
  <head>
    <title>FrontEnd Labs</title>
  </head>
  <body>
    <img src="img1.jpg" alt="Imagen">
  </body>
</html>
```