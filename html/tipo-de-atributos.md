##Tipo de Atributos

No use el tipo de atributos para estilos (al menos que no uses css lo cual es muy poco probable) y tampoco para código javascript (salvo que también utilizes un lenguaje que no sea javascript lo cual es mucho menos probable). Ya que por default trae estos tipos incluso para navegadores antiguos.

>**Ejemplo:**
>```html
<!-- No Recomendado -->
<link rel='stylesheet' href='http://frontend-labs.com/css/admin.css' type='text/css'/>
<!-- Recomendado -->
<link rel='stylesheet' href='http://frontend-labs.com/css/admin.css'/>
<!-- No Recomendado -->
<script type='text/javascript' src='http://frontend-labs.com/js/jquery.js'></script>
<!-- Recomendado -->
<script src='http://frontend-labs.com/js/jquery.js'></script>
```