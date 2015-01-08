##Tipo de Atributos

Use el tipo de atributos para los estilos y también para código javascript . Ya que en algunos navegadores antiguos tanto los estilos como los scrpits no podran ser interpretados por el navegador.

>**Ejemplo:**
>```html
<!-- No Recomendado -->
<script src='http://frontend-labs.com/js/jquery.js'></script>
<link href='http://frontend-labs.com/css/admin.css' rel='stylesheet'/>
```
>```html
<!-- Recomendado -->
<link href="http://frontend-labs.com/css/admin.css" rel="stylesheet" type="text/css"/>
<script src="http://frontend-labs.com/js/jquery.js" type="text/javascript" ></script>
```

