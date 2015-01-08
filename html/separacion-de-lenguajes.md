##Separación de lenguajes
Manten por separado la estructura(html), la presentacion(css) y la conducta (js). La intención es que tus templates solo contengan HTML el cual sirva solo para dar una estructura a la web. Todos los estilos deben estar en otro archivo (css). La conducta de la web no debe presentar datos de estructura, en otras palabras no combines codigo html en tu javascript.

>**Ejemplo:**
>```html
<!-- No recomendado -->
<!DOCTYPE html>
<html>
  <head>
    <title>HTML sucio</title>
    <link href="estilo1.css" media="screen" rel="stylesheet">
    <link href="grilla.css" media="screen" rel="stylesheet">
  </head>
  <body>
    <h1 style="font-size: 1em;">HTML muy sucio</h1>
    <div style="background:red;">tengo mi hoja de estilos pero igual uso estilos en linea</div>
    <script>
      function alertarqueyacargo(){
        alert('la pagina termino de cargar');
      }
    </script>
  </body>
</html>
<!-- Recomendado -->
<!DOCTYPE html>
<html>
  <head>
    <title>HTML Limpio</title>
    <link href="base.css" rel="stylesheet" type="text/css">
  </head>
  <body>
    <h1>HTML Muy limpio</h1>
    <p>Todos los estilos estan en mi hoja de estilos :) </p>
    <script src="funciones.js" type="text/javascript"></script>
  </body>
</html>
```
