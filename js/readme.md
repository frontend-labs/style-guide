
# Guía de estilo Javascript

## Reglas básicas para el uso del patrón modular con YosonJS

Debido a que para el desarrollo de nuestros proyectos utilizamos la librería Javascript: **YosonJS**, hemos desarrollado un documento con las reglas mínimas para codificar un módulo YosonJS y así tener un estándar interno como equipo.


## Reglas

### 1. Todo módulo debe tener una cabecera informativa

Todo módulo YosonJS debe tener una cabecera, compuesta de un comentario multilínea con los siguientes datos básicos:

- Descripción del módulo
- Nombre del módulo
- Nombre del autor

**Ejemplo:**

```js
/*
Descripción del módulo
@module nombre_del_modulo
@author Jan Sanchez 
*/
```

Si el módulo es actualizado por otro miembro del equipo, este debe colocar una coma a continuación del nombre del autor del módulo y luego debe colocar su nombre también.

**Ejemplo:**

```js
/*
Descripción del módulo
@module nombre_del_modulo
@author Jan Sanchez, Carlos Huamaní 
*/
```


### 2.   El nombre del módulo debe estar en "snake_case"

El nombre de un módulo debe estar en `snake_case`. Esto quiere decir que el nombre del modulo debe cumplir las siguientes condiciones:

- Debe estar estrictamente en minúsculas
- Si el nombre del módulo tiene más de una palabra,  debe usarse el símbolo "guión bajo" para unir las palabras siguientes
- No debe contener espacios en blanco

**Ejemplo:**

```js
/*
Descripción del módulo
@module nombre_del_modulo
@author Andres Muñoz 
*/
yOSON.AppCore.addModule ("nombre_del_modulo",  function (Sb) {
  // contenido del módulo
},
["dependencies.js"]);
```



### 3. No poner variables que no se van a usar

En un módulo no se deben declarar variables que no se van a usar.

**Ejemplo:**

```js
/*
Descripción del módulo
@module nombre_del_modulo
@author Ana Reyna, Elizabeth Manrique, Claudia Valdivieso
*/
yOSON.AppCore.addModule ("nombre_del_modulo",  function (Sb) {
  var dom, st, catchDom, events, fn, initialize, suscribeEvents;
  dom = {};
  st = {};
  catchDom = function () {};
  events = function () {};
  fn = function () {};
  suscribeEvents = function () {};  
  initialize = function (oP) {
    $.extend (st, oP);
    catchDom();
    suscribeEvents();
  }
  
  return {
    init: initialize
  } 
},
["dependencies.js"]);
```



### 4. Usar siempre el operador de igualdad estricto === en vez de ==

Se debe utilizar siempre el operador de igualdad estricto `===` en vez de `==`. 

**Ejemplo:**

```js
/*
Descripción del módulo
@module nombre_del_modulo
@author Jhonnatan Castro, Juan Pablo Chullo
*/
yOSON.AppCore.addModule ("nombre_del_modulo",  function (Sb) {
  var dom, st, catchDom, events, fn, initialize, suscribeEvents;
  dom = {};
  st = {};
  catchDom = function () {};
  events = function () {};
  fn = function () {
    getOption = function (){
      var option = false;
      if (window.flag === true) {
        option = window.flag;
      }
      return option;
    }
  };
  suscribeEvents = function () {};  
  initialize = function (oP) {
    $.extend (st, oP);
    catchDom();
    suscribeEvents();
  }
  
  return {
    init: initialize
  } 
},
["dependencies.js"]);
```


### 5. Las nombres de las funciones no deben comenzar con mayúscula

- Los nombres de las funciones de las funciones dentro de un módulo no deben comenzar con una letra mayúscula
- Los nombres de las funciones deben estar en `lowerCamelCase`, como las funciones: `catchDom`, `events`, `fn`, `suscribeEvents` y `initialize` del siguiente ejemplo.

**Ejemplo:**

```js
/*
Descripción del módulo
@module nombre_del_modulo
@author Victor Sandoval, Jhonnatan Castro
*/
yOSON.AppCore.addModule ("nombre_del_modulo",  function (Sb) {
  var dom, st, catchDom, events, fn, initialize, suscribeEvents;
  dom = {};
  st = {};
  catchDom = function () {};
  events = function () {};
  fn = function () {};
  suscribeEvents = function () {};  
  initialize = function (oP) {
    $.extend (st, oP);
    catchDom();
    suscribeEvents();
  }
  
  return {
    init: initialize
  } 
},
["dependencies.js"]);
```


----------





