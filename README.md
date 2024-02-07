--------------

[//]: # (version: 1.0)
[//]: # (author: Fran Dona)
[//]: # (date: 2023-12-07)

--------------

## Vue.js
## Tabla de contenidos
- [VUE.JS](#vuejs-1)
  - [1. Introducción del trabajo](#1-introducción-del-trabajo)
  - [2. ¿Que es Vue.js?](#2-que-es-vuejs)
  - [3. Intalacion de Vue.js](#3-intalacion-de-vuejs)
    - [3.1 Incorporar Vue.js desde CDN](#31-incorporar-vuejs-desde-cdn)
    - [3.2 Incorporar Vue.js para Node.js](#32-incorporar-vuejs-para-nodejs)
      - [3.2.1 Instalación de node.js para Windows](#321-instalación-de-nodejs-para-windows)
      - [3.2.2 Instalación de node.js para Linux](#322-instalación-de-nodejs-para-linux)
      - [3.2.3 Incorporación de Vau.js al proyecto](#323-incorporación-de-vaujs-al-proyecto)
    - [3.3 Incorporación Vue.js medidante CLI](#33-incorporación-vuejs-medidante-cli)
  - [4. Creación de instancias](#4-creación-de-instancias)
    - [4.1 Instancias antiguas (Vue 2.x)](#41-instancias-antiguas-vue-2x)
    - [4.2 Instancias nuevas (Vue 3.X)](#42-instancias-nuevas-vue-3x)
  - [5 Opciones de instancia de Vue](#5-opciones-de-instancia-de-vue)
    - [5.1 data](#51-data)
    - [5.2 methods](#52-methods)
    - [5.3 computed](#53-computed)
    - [5.4 watch](#54-watch)
    - [5.5 props](#55-props)
    - [5.6 emits](#56-emits)
    - [5.7 expose](#57-expose)
  - [6 Incrustaciones de VUE](#6-incrustaciones-de-vue)
  - [7. Directivas de Vue](#7-directivas-de-vue)
    - [7.1 Directiva v-model](#71-directiva-v-model)
      - [7.1.1 Ejemplo v-model](#711-ejemplo-v-model)
    - [7.2 Directiva v-bind](#72-directiva-v-bind)
      - [7.2.1 Ejemplo v-bind](#721-ejemplo-v-bind)
    - [7.3 Directiva v-if, v-else-if, v-else](#73-directiva-v-if-v-else-if-v-else)
      - [7.3.1 Ejemplo v-if, v-else-if, v-else](#731-ejemplo-v-if-v-else-if-v-else)
    - [7.4 Directiva v-for](#74-directiva-v-for)
      - [7.4.1 Ejemplo v-for para texto en listas](#741-ejemplo-v-for-para-texto-en-listas)
      - [7.4.2 Ejemplo v-for para índice en arrays](#742-ejemplo-v-for-para-índice-en-arrays)
      - [7.4.3 Ejemplo v-for para imágenes](#743-ejemplo-v-for-para-imágenes)
      - [7.4.4 Ejemplo v-for para imágenes con texto](#744-ejemplo-v-for-para-imágenes-con-texto)
    - [7.5 Directiva v-on](#75-directiva-v-on)
      - [7.5.1 Ejemplo v-on:input eventos de entrada](#751-ejemplo-v-oninput-eventos-de-entrada)
      - [7.5.2 Ejemplo v-on:mousemove evento movimiento de mause](#752-ejemplo-v-onmousemove-evento-movimiento-de-mause)
      - [7.5.1 Ejemplo v-on:click junto a v-for](#751-ejemplo-v-onclick-junto-a-v-for)
    - [7.6 Directiva v-show](#76-directiva-v-show)
      - [7.6.1 Ejemplo v-show](#761-ejemplo-v-show)
      - [7.6.2 Ejemplo v-show vs v-if](#762-ejemplo-v-show-vs-v-if)
    - [7.7 Directiva v-cloak](#77-directiva-v-cloak)
      - [7.7.1 Ejemplo v-cloak](#771-ejemplo-v-cloak)
    - [7.8 Directiva v-pre](#78-directiva-v-pre)
      - [7.8.1 Ejemplo v-pre](#781-ejemplo-v-pre)
    - [7.9 Directiva v-once](#79-directiva-v-once)
      - [7.9.1 Ejemplo v-once](#791-ejemplo-v-once)
  - [8. Transiciones y Animaciones en Vue.js](#8-transiciones-y-animaciones-en-vuejs)
    - [8.1 Transiciones](#81-transiciones)
    - [8.2 Animaciones](#82-animaciones)
    - [8.3 Ejemplo Práctico](#83-ejemplo-práctico)
  - [9 Creación de un CRUD con VUE.js](#9-creación-de-un-crud-con-vuejs)
  - [10 Ejemplo creación  CRUD](#10-ejemplo-creación--crud)
    - [10.1 Estructura completa del CRUD](#101-estructura-completa-del-crud)
      - [10.1.1 Parte HTML del CRUD](#1011-parte-html-del-crud)
      - [10.1.2 Parte VUE.js del CRUD](#1012-parte-vuejs-del-crud)
  - [11 CRUD paso a paso](#11-crud-paso-a-paso)
    - [11.1 Crear (Create)](#111-crear-create)
    - [11.2 Leer (Read)](#112-leer-read)
    - [11.3 Actualizar (Update)](#113-actualizar-update)
    - [11.4 Borrar (Delete)](#114-borrar-delete)
  - [12 ¿Que es vuex?](#12-que-es-vuex)
  - [12.1 Principales Conceptos en Vuex:](#121-principales-conceptos-en-vuex)
    - [12.1.1 Estado (State):](#1211-estado-state)
    - [12.1.2  Mutaciones (Mutations):](#1212--mutaciones-mutations)
    - [12.1.3  Acciones (Actions):](#1213--acciones-actions)
    - [12.1.4 Getters:](#1214-getters)
    - [12.1.5 Módulos:](#1215-módulos)
  - [12.2 Vuex es beneficioso cuando:](#122-vuex-es-beneficioso-cuando)
  - [13. Vue Router](#13-vue-router)
    - [13.1 Rutas (Routes)](#131-rutas-routes)
    - [13.2 Enrrutamiento Anidado](#132-enrrutamiento-anidado)
    - [13.3 Navegacion Programática](#133-navegacion-programática)
    - [13.4 Parámetros de ruta](#134-parámetros-de-ruta)
    - [13.5 Transiciones de Vista](#135-transiciones-de-vista)
    - [13.6 Guardias de Navegación](#136-guardias-de-navegación)
    - [13.7 Modo de Historial](#137-modo-de-historial)
    - [13.8 Lazy Loading de COmponentes](#138-lazy-loading-de-componentes)
  - [14. Mantenimiento y Escalabilidad](#14-mantenimiento-y-escalabilidad)
  - [15. Fuentes](#15-fuentes)

<div style="page-break-after: always;"></div>

# VUE.JS

## 1. Introducción del trabajo
[Índice](#tabla-de-contenidos)

En este documento, exploraremos diversas **utilidades de Vue.js**, abarcando desde su proceso de **instalación** hasta la **creación de proyectos sencillos**. Además, analizaremos conceptos fundamentales como la **creación de componentes** y la gestión de estado mediante VueX. Este recurso servirá como guía integral para aquellos que deseen iniciarse con Vue.js y aprovechar al máximo su potencial en el desarrollo de aplicaciones web modernas.

## 2. ¿Que es Vue.js?
[Índice](#tabla-de-contenidos)

Vue.js es un **framework** progresivo de JavaScript que se destaca por su enfoque **reactivo**, facilitando la construcción de **interfaces** de usuario **interactivas** y de una sola página (SPA). Su estructura modular simplifica el desarrollo de aplicaciones web modernas, con una curva de aprendizaje suave. Vue.js se integra fácilmente en proyectos existentes y permite crear **páginas responsivas** con menos código que los métodos tradicionales de JavaScript. En nuestro caso, utilizaremos Vue para controlar y manejar la lógica de una parte específica de la interfaz de usuario.

## 3. Intalacion de Vue.js
[Índice](#tabla-de-contenidos)

Tenemos varios tipos de incluir Vue.js a nuestro proyecto
Tenemos dos tipos de 
(En todos los casos usaremos la version de produccion y no la de desarroyo para asegurarnos que no da problemas)

### 3.1 Incorporar Vue.js desde CDN
> Serán los mismos pasos para windows y linux

<br>
Metodo mas sencillo y comun

```html
<script src="https://unpkg.com/vue@3/dist/vue.global.js"> </script>
```
<br>
También podemos acceder al link https://es.vuejs.org/js/vue.min.js y guardar el .js directamente en nuestros archivos locales del servidor.

```html
<script src="archivos/vue.js"></script>
```
<div style="page-break-after: always;"></div>

### 3.2 Incorporar Vue.js para Node.js



#### 3.2.1 Instalación de node.js para Windows
[Índice](#tabla-de-contenidos)

 1. Para instalar Node en nuestro Windows nos dirigiremos a la pagina oficial y descargaremos la versión que necesitemos https://nodejs.org/en
 2. Comprobaremos que esta instalado y funcionando yendo al cmd o PowerShell y ejecutando el siguiente comando.

``` PowerShell
  node -v
  npm -v
```
#### 3.2.2 Instalación de node.js para Linux
[Índice](#tabla-de-contenidos)


- En el caso de linux será algo mas sencillo  
  1. Nos dirigiremos al terminal y empezaremos la instalación, tendremos dos opciones mediante la instalación tradicional o por cur
   <br><br>
 - Instalación tradicional

  
```bash
  sudo apt update
  sudo apt install nodejs npm
```

 - Curl

```bash
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
  nvm install node
```

<div style="page-break-after: always;"></div>

#### 3.2.3 Incorporación de Vau.js al proyecto
[Índice](#tabla-de-contenidos)


1. Crearemos un proyecto de node en donde queramos y entraremos a la carpeta
```bash
mkdir proyecto-vue
cd proyecto-vue
```

1.1 Inicializaremos el proyecto con el siguiente comando

```bash
npm init -y
```

2. Instalaremos Express con el siguiente comando para facilitar la creación  de la aplicación
   
```bash
npm install express
```

3. Crearemos un servidor express para visualizar nuestro proyecto mas fácilmente
   
```javascript
// app-vue.js
const express = require('express');
const app = express();
const port = 3000;

app.get('/', (req, res) => {
  res.send('Hola, mundo!');
});

app.listen(port, () => {
  console.log(`Servidor escuchando en http://localhost:${port}`);
});
```

4. Instalamos vue en nuestro proyecto

```bash
npm install vue
```

<div style="page-break-after: always;"></div>

5. Crearemos un archivo html en una carpeta a parte que será la donde almacenemos archivos html estáticos

```bash
mkdir paginas
```
<br>

5.1 Crearemos un archivo html 

```html
<!-- pagina/index.html -->
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mi Aplicación Vue</title>
</head>
<body>

  <script src="https://cdn.jsdelivr.net/npm/vue@2"></script>
  <script src="/js/main.js"></script>

  <div id="app">
    {{ message }}
  </div>


</body>
</html>

```
6. Crearemos una carpeta nueva para almacenar las instancias de vue con un ejemplo muy básico
   
```javascript
// public/js/main.js
import { createApp } from 'vue';
const app = createApp({
  data() {
    return {
      message: '¡Hola, Mundo!'
    };
  }
});

app.mount('#app');   
```

<div style="page-break-after: always;"></div>

7. Terminaremos de configurar el archivo de Express
```javascript
// app.js
const express = require('express');
const app = express();
const port = 3000;

// Configurar middleware para servir archivos estáticos
app.use(express.static('paginas'));

app.get('/', (req, res) => {
  res.sendFile(__dirname + '/public/index.html');
});

app.listen(port, () => {
  console.log(`Servidor escuchando en http://localhost:${port}`);
});
```

8. Para finalizar iniciaremos el proyecto y comprobaremos que todo funciona
```bash
node app-vue.jsa
```


-----

### 3.3 Incorporación Vue.js medidante CLI
[Índice](#tabla-de-contenidos)
> Serán los mismos pasos para windows y linux

1. Empezaremos instalando Vue CLI
  ```bash
  npm install -g @vue/cli
  ```

2. Crearemos un proyecto nuevo
  ```bash
  vue create proyecto-vue
  ```
3. Nos movemos al proyecto que hemos creado
  ```bash
  cd proyecto-vue
  ```

<div style="page-break-after: always;"></div>

4. Por ultimo ejecutaremos la aplicación
  ```bash
  npm run serve
  ```

  Esto iniciara la aplicación en un servidor de desarrollo al cual podremos acceder poniendo http://localhost:8080 en el navegador


5. Por ultimo podremos comenzar con el proyecto y modificar los archivos en el directorio "src".



## 4. Creación de instancias

 Una instancia de Vue es un objeto que representa y controla una parte específica de la interfaz de usuario. Está asociada a un elemento HTML y contiene la lógica y los datos para ese elemento.

  - Dependiendo de la versión de vue que usemos tenemos dos opciones de crear instancias, aquí veremos las dos, ya que esta la posibilidad de encontrárnoslo, pero recomiendo usar siempre la nueva.

> En todos los casos será igual para Linux y Windows

- En los siguientes ejemplos los datos que contendrán las instancias serán solo un mensaje que mostraremos en pantalla

  <div style="page-break-after: always;"></div>

  ### 4.1 Instancias antiguas (Vue 2.x)

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vue 2.X Instance</title>
  <script src="https://cdn.jsdelivr.net/npm/vue@2"></script>
</head>
  <body>

    <div id="app">
      {{ mensaje }}
    </div>


    
    <script>
      // Instamcia de Vue
      var app = new Vue({
        el: '#app',
        data: {
          mensaje: '¡Hola mundo desde Vue 2.X!'
        }
      });
    </script>

</body>
</html>
```

<br>

> En Vue.js 2.0, una instancia se crea con new Vue({}). La instancia se vincula a un elemento del DOM con el. La propiedad data define los datos reactivos, como mensaje. La expresión {{ mensaje }} en el DOM establece una vinculación de datos bidireccional: cualquier cambio en mensaje se refleja en el DOM y viceversa. Las instancias también pueden tener métodos y eventos. En resumen, Vue.js 2.0 utiliza instancias para gestionar la reactividad y la lógica de una sección específica de la interfaz de usuario.

  <div style="page-break-after: always;"></div>
  
  ### 4.2 Instancias nuevas (Vue 3.X)

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <title>My first Vue page</title>
</head>
<body>

  <div id="app">
    {{ mensaje }}
  </div>

  <script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>

  <script>
    const app = Vue.createApp({
      data() {
        return {
          mensaje: "Hola mundo, desde Vue 3.X!"
        }
      }
    })

   app.mount('#app')

  </script>
</body>
</html>
```

<br>

> Vue.createApp: En Vue.js 3.0, se utiliza Vue.createApp para crear una aplicación en lugar de new Vue.
data() en lugar de data: En la definición del componente, data ahora se define como una función que devuelve un objeto.
app.mount('#app'): La aplicación se monta en un elemento del DOM utilizando el método mount. En lugar de especificar el como en Vue.js 2.0, ahora se utiliza mount para montar la aplicación en un selector específico.
Estos cambios reflejan la nueva sintaxis y la estructura de Vue.js 3.0, que está diseñada para mejorar la eficiencia y la legibilidad del código.

<div style="page-break-after: always;"></div>


## 5 Opciones de instancia de Vue

### 5.1 data
[Índice](#tabla-de-contenidos)
```html
<article>
  <h2>Opción de Datos de Ejemplo</h2>
  <p>Utilizando la propiedad de datos 'msg' dentro de la opción de datos para almacenar un mensaje:</p>
  <pre>{{ msg }}</pre>
</article>

<script>
export default {
  data() {
    return {
      msg: '¡Hola Mundo!'
    };
  }
};
</script>
```
>Este código utiliza la opción data para definir una propiedad llamada msg que almacena el mensaje "¡Hola Mundo!". La propiedad msg se puede utilizar en la plantilla para mostrar el mensaje.

> **data:** En Vue.js se usa para almacenar datos reactivos en un componente, permitiendo que la interfaz de usuario se actualice automáticamente cuando estos datos cambian.


<div style="page-break-after: always;"></div>


### 5.2 methods
[Índice](#tabla-de-contenidos)
```html
<article>
  <h2>Opción de Ejemplo para Métodos</h2>
  <p>Utilizando el método 'toggleMsg' dentro de la opción de métodos para alternar un mensaje:</p>
  <button v-on:click="toggleMsg">Alternar Mensaje</button>
  <pre v-show="showMsg">{{ msg }}</pre>
</article>

<script>
export default {
  data() {
    return {
      msg: '¡Hola Mundo!',
      showMsg: false
    };
  },
  methods: {
    toggleMsg() {
      this.showMsg = !this.showMsg;
    }
  }
};
</script>

```

>Este código utiliza la opción methods para definir un método llamado toggleMsg que alterna el valor de showMsg al hacer clic en un botón.

>**methods:** En Vue.js se usa para definir funciones en un componente, permitiendo la encapsulación de la lógica y acciones específicas que responden a eventos o interacciones del usuario.

-------

<div style="page-break-after: always;"></div>

### 5.3 computed
[Índice](#tabla-de-contenidos)
```html
<article>
  <h2>Opción de Ejemplo para Propiedades Calculadas</h2>
  <p>Utilizando el valor calculado 'btnText' dentro de la opción de propiedades calculadas para mostrar el texto de botón apropiado:</p>
  <button v-on:click="this.showMsg = !this.showMsg">
    {{ btnText }}
  </button>
  <pre v-show="showMsg">{{ msg }}</pre>
</article>

<script>
export default {
  data() {
    return {
      msg: '¡Hola Mundo!',
      showMsg: false
    };
  },
  computed: {
    btnText() {
      if (this.showMsg) {
        return 'Ocultar';
      } else {
        return 'Mostrar';
      }
    }
  }
};
</script>
```

>Este código utiliza propiedades calculadas (computed) para generar el texto del botón (btnText) de manera más concisa. Si showMsg es true, devuelve 'Hide', de lo contrario, devuelve 'Show'.

>**computed:** En Vue.js se usa para crear propiedades que se calculan automáticamente según datos reactivos en el componente. En el código, se utiliza para simplificar la lógica de generación del texto del botón (btnText).

------

<div style="page-break-after: always;"></div>


### 5.4 watch
[Índice](#tabla-de-contenidos)
```html
<template>
  <h2>Opción de ejemplo de watcher</h2>
  <p>Utilizando el watcher 'rangeVal' dentro de la opción de watch para que no se puedan elegir valores entre 20 y 70:</p>
  <input type="range" v-model="rangeVal">
  <p>rangeVal: <span>{{ rangeVal }}</span></p>
</template>

<script>
export default {
  data() {
    return {
      rangeVal: 4
    };
  },
  watch: {
    rangeVal(val) {
      if (val > 20 && val < 70) {
        if (val < 40) {
          this.rangeVal = 20;
        } else {
          this.rangeVal = 70;
        }
      }
    }
  }
};
</script>
```

>**watch** en este código usa un para asegurar que los valores del rango (rangeVal) estén restringidos entre 20 y 70. Si el valor está fuera de ese rango, se ajusta automáticamente al límite más cercano.

>**watch:** En Vue.js se utiliza para observar cambios en los datos y realizar acciones específicas cuando esos cambios ocurren, proporcionando una forma de responder a cambios en las propiedades de datos y realizar lógica personalizada en consecuencia.

<div style="page-break-after: always;"></div>


### 5.5 props
[Índice](#tabla-de-contenidos)
```html
<article>
    <div>
        <h2>{{ foodName }}</h2>
        <p>{{ foodDesc }}</p>
    </div>
</article>

<script>
export default {
    props: [
        'foodName',
        'foodDesc'
    ]
};
</script>
```
>**props** en este código define que el componente espera recibir dos propiedades, foodName y foodDesc, que pueden ser proporcionadas por el componente padre y se utilizan para mostrar datos dentro del componente hijo.

>**props:** en Vue.js son atributos personalizados que permiten la comunicación de datos unidireccional desde el componente padre al hijo. En el código, foodName y foodDesc son propiedades que se pueden pasar al componente desde su componente padre.

------

<div style="page-break-after: always;"></div>

### 5.6 emits
[Índice](#tabla-de-contenidos)
```html
<article>
  <div>
    <h3>ChildComp.vue</h3>
    <p>Haz clic en el botón para activar el evento personalizado con el mensaje "¡Hola!" hacia el componente padre utilizando el método $emit().</p>
    <button v-on:click="notifyParent">Activar</button>
  </div>
</article>

<script>
export default {
  emits: ['custom-event'],
  methods: {
    notifyParent() {
      this.$emit('custom-event', '¡Hola! ')
    }
  }
}
</script>
```

>**emits: ['custom-event']** permite al componente hijo emitir el evento personalizado 'custom-event'. Al hacer clic en el botón, se utiliza this.$emit('custom-event', '¡Hola! ') para enviar el mensaje '¡Hola!' al componente padre.

>**emits** en Vue.js se usa para especificar qué eventos personalizados puede emitir un componente hijo. En el código proporcionado, emits: ['custom-event'] permite al componente hijo enviar un evento personalizado llamado 'custom-event' al componente padre.

<div style="page-break-after: always;"></div>


### 5.7 expose
[Índice](#tabla-de-contenidos)
```html
<article>
  <div>
    <p>Mensaje del componente padre:</p>
    <p id="pEl">{{ message }}</p>
  </div>
</article>

<script>
export default {
  expose: ['createMessage'],
  data() {
    return {
      message: ' '
    }
  },
  methods: {
    createMessage(msg) {
      this.message += msg + ' '
    }
  }
}
</script>
```

>**expose:** En este casao lo utilizamos para exponer métodos o propiedades específicas del componente hijo a su componente padre. En este caso, expose: ['createMessage'] permite que el componente padre llame al método createMessage del componente hijo.

>**expose:** En Vue.js se utiliza para permitir que un componente hijo exponga métodos o propiedades específicas para que puedan ser utilizadas por su componente padre. Facilita la comunicación controlada entre componentes.

<div style="page-break-after: always;"></div>


## 6 Incrustaciones de VUE

Las instancias de VUE no tienen por que estar completamente visibles en el documento HTML, podemos crear instancias en archivos externos y vincularlos al documento como si fuese un css.

Documentos/<br>
|-- instancia.js<br>
|-- index.html<br>

```js
//instancia.js
const app = Vue.createApp({
  data() {
    return {
      manuales: [
        'https://shorturl.at/rAENV',
        'https://shorturl.at/ijuvw',
        'https://shorturl.at/amEI0',
      ]
    }
  }
  })
  
  app.mount('#app')
```
```html
<!-- index.html -->
<body>
<div id="app">
  <div>
    <img v-for="x in manuales" v-bind:src="x" width="70" height="100">
  </div>
</div>
  <script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
  <!-- Incorporación de la instancia -->
  <script src="instacia.js"></script> 
</body>
</html>
```

## 7. Directivas de Vue

Las directivas de Vue son atributos especiales que se añaden a las etiquetas HTML para establecer una conexión dinámica con las instancias de Vue. Estas directivas permiten crear interfaces más interactivas y dinámicas para los usuarios al proporcionar funcionalidades especiales que afectan el comportamiento o la presentación de los elementos HTML asociados.

A continuación vamos a ver las directivas que más se usan:

  <div style="page-break-after: always;"></div>

### 7.1 Directiva v-model
**v-model:** Se utiliza para crear enlaces bidireccionales en formularios. Enlaza automáticamente la entrada del usuario a una propiedad en el modelo.


```html
<input v-model="message">
```

#### 7.1.1 Ejemplo v-model

```html
<body>

<div id="app">
  <p> De acuerdo! Su nombre es: [{{ nombre }}] y tienes [{{ edad }}] años</p>
  <br>
  Digame su nombre <input v-model="nombre" placeholder="Nombre">
<br><br>
  Digame su edad <input v-model="edad" placeholder="edad">
</div>

<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
<script>
    const app = Vue.createApp({
      data() {
        return {
          nombre: '',
          edad: '',
        };
      }
    });
  
    app.mount('#app');
  </script>

</body>
```
> **v-model** en este código establece un enlace bidireccional entre las propiedades nombre y edad en la instancia de Vue y el valor de un elemento < input > en el HTML. Esto implica que cualquier cambio en el < input > se reflejará automáticamente en las propiedades de Vue, y viceversa. En esencia, v-model simplifica la sincronización automática entre los datos en el modelo de Vue y los elementos de la interfaz de usuario.

--------

  <div style="page-break-after: always;"></div>

### 7.2 Directiva v-bind
**v-bind:** Se utiliza para enlazar un atributo o una propiedad del elemento HTML a una expresión de Vue.


```html
<div v-bind:[attribute]="[Vue data]"></div>
```
<br>

#### 7.2.1 Ejemplo v-bind

```html
<body>

  <div id="app" v-bind:style="estilo">
    <img v-bind:src="url">
    <a v-bind:href="link">Link para ver manuales de Vue</a>
  </div>
  

<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
<script>
  const app = Vue.createApp({
    data() {
      return {
        url: 'https://shorturl.at/ahGK5',
        link: 'https://shorturl.at/lwG06',
      }
    }
  })
  app.mount('#app');
  </script>

</body>
```
> **v-bind** se esta usando para enlazar dinámicamente los valores de las 
  propiedades url y link a los atributos src y href en los 
  elementos < img > y < a >. Esto permite que la imagen y el 
    enlace cambien de manera reactiva según los datos definidos 
    en tu instancia de Vue.
--------

  <div style="page-break-after: always;"></div>

### 7.3 Directiva v-if, v-else-if, v-else

**v-if, v-else-if, v-else:** Estas directivas condicionales permiten mostrar u ocultar elementos basados en expresiones condicionales.

```html
<p v-if="seen">Ahora me ves</p>
<p v-else>No me ves</p>
```
<br>

#### 7.3.1 Ejemplo v-if, v-else-if, v-else

```html
<body>

<h2>Venta de Manuales HTML</h2>
<img src="https://shorturl.at/rAENV" alt="manual" width="120" height="135">

<div id="app">
  <p v-if="contadorManuales>3">
    En stock
  </p>
  <p v-else-if="contadorManuales>0">
    ¡Quedan muy pocos!
  </p>
  <p v-else>
    Sin stock
  </p>
</div>

<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
<script>
  const app = Vue.createApp({
    data() {
    return {
      contadorManuales: 4
    }
    }
  })
  app.mount('#app')
</script>

</body>
```
> **v-if, v-else-if, v-else:** En este ejemplo del inventario de una tienda
podemos ver como hemos configurado las 3 directivas para dependiendo del datos
de salida de la estancia nos de una respuesta diferente 

--------

<div style="page-break-after: always;"></div>

### 7.4 Directiva v-for
**v-for:** Se utiliza para realizar bucles a través de una matriz o un objeto y renderizar elementos múltiples.

```html
<ul>
  <li v-for="item in items">{{ item.text }}</li>
</ul>
```
<br>


#### 7.4.1 Ejemplo v-for para texto en listas

```html
<body>

<div id="app">

  <ol>
    <li v-for="x in manyFoods">{{ x }}</li>
  </ol>

</div>

<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>

<script>
  const app = Vue.createApp({
  data() {
    return {
      manyFoods: [
        'Manual HTML',
        'Manual CS',
        'Manual JavaScript',
      ]
    }
  }
  })
  
  app.mount('#app')

</script>

</body>
```
> **v-for:** En este ejemplo, 'v-for' crea un 'li' etiqueta con el nombre del manual para cada manual en el array de la instancias de Vue
--------

<div style="page-break-after: always;"></div>

#### 7.4.2 Ejemplo v-for para índice en arrays

```html
<body>
<h1>Ejemplo Obtener el índice del elemento del arrays con 'v-for'</h1>

<div id="app">
  <div>
    <p v-for="(x, index) in manuales">
      {{ index }}: "{{ x }}" <br>
    </p>
  </div>
</div>

<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
<script>
  const app = Vue.createApp({
  data() {
    return {
      manuales: [
        'Manual HTML',
        'Manual CSS',
        'Manual JavaScript',
        'Manual Java',
        'Manual ',
      ]
    }
  }
  })
  app.mount('#app')
</script>

</body>
```
> **v-for:** se utiliza para obtener el índice y el nombre 
  de los elementos dentro de la matriz 'manuales' en la instancia de Vue.
  
-------

<div style="page-break-after: always;"></div>

#### 7.4.3 Ejemplo v-for para imágenes

```html
<h1>Ejemplo con 'v-for' para crear imágenes</h1>

<div id="app">

  <div>
    <img v-for="x in manuales" v-bind:src="x" width="70" height="100">
  </div>

</div>

<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>

<script>
  const app = Vue.createApp({
  data() {
    return {
      manuales: [
        'https://shorturl.at/rAENV',
        'https://shorturl.at/ijuvw',
        'https://shorturl.at/amEI0',

      ]
    }
  }
  })
  
  app.mount('#app')

</script>
```

> **v-for:** Con esta función podremos imprimir en pantalla arrays que declaremos dentro de la instancia de vue, en este caso lo hemos hecho con un conjunto de imágenes

--------

<div style="page-break-after: always;"></div>

#### 7.4.4 Ejemplo v-for para imágenes con texto

```html
<body>

<h1>Ejemplo 'v-for' Para crear imágenes con texto</h1>

<div id="app">
  <div>
    <figure v-for="x in manuales">
      <img v-bind:src="x.url" width="100" height="100">
      <figcaption>{{ x.nombre }}</figcaption>
    </figure>
  </div>
  

</div>

<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>

<script>
  const app = Vue.createApp({
   data() {
    return {
      manuales: [
        {nombre: 'Manual HTML', url: 'https://shorturl.at/rAENV'},
        {nombre: 'Manual CSS', url: 'https://shorturl.at/ijuvw'},
        {nombre: 'Manual JavaScript', url: 'https://shorturl.at/amEI0'},
      ]
    }
   }
  })
  
  app.mount('#app')

</script>
</body>
```
> **v-for:** Será igual que al declarar imágenes pero podemos 
  añadirle texto a cada imagen individualmente

--------

<div style="page-break-after: always;"></div>

### 7.5 Directiva v-on
**v-on o @:** Se utiliza para escuchar eventos y ejecutar métodos de Vue cuando esos eventos ocurren.

```html
<button v-on:click="doSomething">Haz algo</button>
<!-- O usando la forma corta con @ -->
<button @click="doSomething">Haz algo</button>
```
<br>

#### 7.5.1 Ejemplo v-on:input eventos de entrada

```html

<body>
<h1>Ejemplo: Contador de eventos</h1>

<div id="app">
  <input type="text" v-on:input="contadoreventos++" placeholder="Start writing..">
  <p>{{ 'Input events occured: '+contadoreventos }}</p>
</div>

<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
<script>
  const app = Vue.createApp({
    data() {
      return {
        contadoreventos: 0
      }
    }
  })
 app.mount('#app')

</script>
</body>

```
>**v-on:** Esta escuchando el evento de entrada
en el campo de texto, el "contadoreventos++" incrementa
el contador cada vez que ocurre un evento y la respuesta
de la estancia de vue lo que hacer es mostrar los 
eventos en pantalla

--------

<div style="page-break-after: always;"></div>

#### 7.5.2 Ejemplo v-on:mousemove evento movimiento de mause

```html
<body>

<h1>Example: Change Color</h1>

<div id="app">
  <div v-on:mousemove=" valorcolor = Math.floor(Math.random()*360) " v-bind:style=" {backgroundColor: 'hsl('+valorcolor+',60%,60%)'} "></div>
  <p><span>backgroundColor: hsl(<strong>{{ valorcolor }}</strong>, 80%, 80%)</span></p>
</div>

<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
<script>
  const app = Vue.createApp({
    data() {
      return {
        valorcolor: 50
      }
    }
  })
 app.mount('#app')
</script>

</body>
```

>**v-on:mausemove:** Hemos creado una estancia llamada app 
con un valor asociado, dentro del div hemos creado
el evento de mausemove, cuando el valorcolor cambia,
hace que cambie el valor hsl de fondo, por lo que cambia
de color. Dependiendo del valor que establezcamos en
la estancia será el color predeterminado con el que cargara la página.

--------

<div style="page-break-after: always;"></div>

#### 7.5.1 Ejemplo v-on:click junto a v-for

```html
<body>

<h1>Ejemplo: v-on con v-for</h1>

<div id="app">
  <ol>
    <li v-for="manuales in masmanuales" v-on:click="urlImagen = manuales.url">
      {{ manuales.nombre }}
    </li>
  </ol>
  <img v-bind:src="urlImagen" width="120">
</div>

<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
<script>
  const app = Vue.createApp({
    data() {
      return {
        urlImagen: 'https://shorturl.at/rAENV',
        masmanuales: [
          {nombre: 'HTML', url: 'https://shorturl.at/rAENV'},
          {nombre: 'CSS', url: 'https://shorturl.at/ijuvw'},
          {nombre: 'JS', url: 'https://shorturl.at/amEI0'},
        ]
      }
    }
  })
app.mount('#app')
</script>

</body>
```
>**v-on:click:** En este código estamos creando una lista con v-for recogiendo los datos de la estancia creada con vue y con v-on:click hacemos que la lista sea clicable de esta manera podemos cambiar la imagen que tenemos en los datos de la estancia

--------

<div style="page-break-after: always;"></div>

### 7.6 Directiva v-show
**v-show:** Similar a v-if, pero en lugar de agregar o quitar elementos del DOM, simplemente oculta o muestra el elemento con CSS.

```html
<p v-show="seen">Ahora me ves</p>
```
<br>

#### 7.6.1 Ejemplo v-show

```html
<head>
  <title>v-show</title>
  <style>
    #app div {
      width: 100px;
      padding: 20px;
      background-color: rgb(63, 0, 253);
      font-weight: bold;
    }
  </style>
</head>
<body>

<h1>Ejemplo: v-show</h1>
<div id="app">
  <div v-show="visibilidad">Este mensaje solo puede verse si "visibilidad" es verdadero </div>
</div>

<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
<script>
  const app = Vue.createApp({
    data() {
      return {
        visibilidad: true
      }
    }
  })
app.mount('#app')
</script>
</body>
```
>**v-show:** Al cambia el valor de "visibilidad" dentro de la instancia de vue, entre falso y verdadero el elemento que tenga la propiedad, en este caso el div, será visible o no.

--------

<div style="page-break-after: always;"></div>

#### 7.6.2 Ejemplo v-show vs v-if

```html
<body>
<h1>Ejemplo: v-show vs v-if</h1>

<div id="app">
  <p>Establezca la propiedad de datos 'visualizar' en 'false' y vuelva 
    a ejecutar el código. Haga clic con el botón derecho en este elemento 
    p verde, elija 'Inspeccionar elemento' y podrá ver 
    que el elemento div con v-show todavía existe, solo es la propiedad 
    de visualización CSS la que se establece en 'none', y el div con v-if 
    se destruye.</p>
  <div v-show="visualizar">Div tag with v-show</div>
  <div v-if="visualizar">Div tag with v-if</div>
</div>

<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
<script>
  const app = Vue.createApp({
    data() {
      return {
        visualizar: true
      }
    }
  })
 app.mount('#app')
</script>

</body>
```
>**v-show:** aunque el elemento v-show se haya oculta sigue existiendo en vez de destruirlo
de esta manera, si estamos en una página que cambie mucho su estado será preferible para mejorar
el rendimiento.

Si estamos en una página que no cambia mucho el estado podremos usar v-if

--------

<div style="page-break-after: always;"></div>

### 7.7 Directiva v-cloak
**v-cloak:** Se utiliza para evitar que las expresiones de Vue se muestren antes de que se hayan compilado.

```html
<div v-cloak>
  {{ message }}
</div>
```

> v-cloak está desfasado desde que apareció en la versión 3 de vue, pero todavía se puede encontrar en algún código por lo que es bueno saber cómo funciona para no sorprendernos cuando lo veamos.

<br>

#### 7.7.1 Ejemplo v-cloak


```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vue.js 3 Example</title>
  <script src="https://unpkg.com/vue@3"></script>
</head>
<body>

<div id="app">
  <div v-if="dataLoaded">
    <h1>{{ responseData.title }}</h1>
    <p>{{ responseData.content }}</p>
  </div>
  <div v-else>
    Cargando datos...
  </div>
</div>

<script>
// Define el componente Vue
const app = Vue.createApp({
  data() {
    return {
      dataLoaded: false,
      responseData: null
    };
  },
  mounted() {
    setTimeout(() => {
      this.responseData = {
        title: 'Título de ejemplo',
        content: 'Contenido de ejemplo'
      };
      this.dataLoaded = true; 
    }, 2000);
  }
});
app.mount('#app');
</script>

</body>
</html>
```
<br><br>
>La función v-cloak de Vue.js fue introducida en versiones anteriores (Vue.js 2 y anteriores) como una manera de evitar que el contenido visible en la página parpadee antes de que Vue.js tenga la oportunidad de interpretar las directivas y realizar la vinculación de datos.
Sin embargo, con las mejoras introducidas en Vue.js 3, se ha trabajado para mejorar el manejo de este comportamiento. En Vue.js 3, el sistema de reactividad y la forma en que se maneja la inicialización de los componentes han sido mejorados para abordar este problema de parpadeo sin la necesidad de v-cloak.

--------

<div style="page-break-after: always;"></div>

### 7.8 Directiva v-pre
**v-pre:** Muestra el texto sin compilar dentro del elemento. Útil cuando se quiere mostrar código Vue sin que se interprete.

```html
<span v-pre>{{ This will not be compiled }}</span>
```
<br>

#### 7.8.1 Ejemplo v-pre

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejemplo v-pre</title>
</head>
<body>

    <h1>Ejemplo: v-pre</h1>
    
    <div id="app" v-pre>
      {{ mensaje }}
    </div>
    
    <script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
    <script>
      const app = Vue.createApp({
        data() {
          return {
            mensaje: 'Este es un mensaje que no será compilado por Vue.'
          };
        }
      });

      app.mount('#app');
    </script>
</body>
</html>
```
> **v-pre:** funciona de manera que desactiva la compilación del contenido
dentro del elemento. Se usa cuando se desea 
mostrar código Vue sin procesamiento.

--------

<div style="page-break-after: always;"></div>


### 7.9 Directiva v-once
**v-once:** Renderiza el elemento o la plantilla solo una vez.

```html
<h1 v-once>{{ title }}</h1>
```
<br>

#### 7.9.1 Ejemplo v-once

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vue 3 v-once Ejemplo</title>
  
</head>
<body>

<div id="app">
  <h1 v-once>{{ mensaje }}</h1>
</div>
<script src="https://cdn.jsdelivr.net/npm/vue@3"></script>
<script>
  const app = Vue.createApp({
    data() {
      return {
        mensaje: '¡Hola, este mensaje solo se renderizará una vez en Vue 3!'
      };
    }
  });
  const vm = app.mount('#app');
</script>

</body>
</html>
```
> **v-once:** Hace que solo se renderice una vez de manera que si se intentan actualizar los datos no cambiaran. Esto puede ser útil cuando tienes partes de tu interfaz de usuario que no necesitan ser reevaluadas en cada cambio de estado, mejorando así el rendimiento al reducir la cantidad de actualizaciones en el DOM.


--------

<div style="page-break-after: always;"></div>

## 8. Transiciones y Animaciones en Vue.js

### 8.1 Transiciones

En Vue.js, las transiciones permiten agregar efectos suaves a los cambios en el DOM, como la entrada o salida de elementos. Puedes utilizar las clases de CSS predefinidas para controlar estos efectos.

```html
<transition name="fade">
  <p v-if="mostrar">¡Hola, soy un elemento con transición!</p>
</transition>
```

```css
.fade-enter-active, .fade-leave-active {
  transition: opacity 0.5s;
}
.fade-enter, .fade-leave-to {
  opacity: 0;
}
```

### 8.2 Animaciones

Las animaciones en Vue.js van más allá de las transiciones y te permiten crear efectos más complejos y personalizados. Puedes definir animaciones usando @keyframes en CSS y luego aplicarlas en Vue.

```html
<transition name="custom-animation">
  <p v-if="mostrar" class="animate">¡Hola, soy un elemento animado!</p>
</transition>
```

```css
@keyframes custom-animation {
  from { transform: translateX(-100%); }
  to { transform: translateX(0); }
}

.custom-animation-enter-active, .custom-animation-leave-active {
  animation: custom-animation 1s;
}
.custom-animation-enter, .custom-animation-leave-to {
  transform: translateX(0);
}
```

<div style="page-break-after: always;"></div>


### 8.3 Ejemplo Práctico

Supongamos que tienes un botón que muestra u oculta un elemento con una transición:



```html
<template>
  <div>
    <button @click="toggleElement">Mostrar/Ocultar Elemento</button>
    <transition name="fade">
      <p v-if="mostrar">¡Hola, soy un elemento con transición!</p>
    </transition>
  </div>
</template>

<script>
export default {
  data() {
    return {
      mostrar: false
    };
  },
  methods: {
    toggleElement() {
      this.mostrar = !this.mostrar;
    }
  }
};
</script>

<style>
.fade-enter-active, .fade-leave-active {
  transition: opacity 0.5s;
}
.fade-enter, .fade-leave-to {
  opacity: 0;
}
</style>

```



<div style="page-break-after: always;"></div>

## 9 Creación de un CRUD con VUE.js

A continuación, vamos a ver un ejemplo completo y luego explicado paso a paso en el que hemos creado un CRUD para gestión datos de unos clientes.
Podremos ver los cuatro fundamentos básicos del CRUD: Create, Read, Update, Delete.
El ejemplo completo seria asi:


## 10 Ejemplo creación  CRUD

### 10.1 Estructura completa del CRUD

#### 10.1.1 Parte HTML del CRUD
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Pacientes</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.0/css/bootstrap.min.css">
    <script src="https://unpkg.com/vue@3"></script>
</head>
<body>
  <div id="appPacientes" class="container">
    <!-- Formulario para añadir pacientes -->
    <section class="form">
      <form action="" class="text-center">
        <input v-model="nombre" @keyup.enter="crearPaciente" type="text" class="form-control"eholder="Nombre">
        <input v-model="edad" @keyup.enter="crearPaciente" type="number" name="edad" placeholder="Edad" class="form-control">
        <!-- Botón para añadir -->           
        <input @click="crearPaciente" type="button" value="Añadir"class="btn btn-success">
      </form>
    </section>
    <!-- Tabla donde se muestran los datos -->
    <section class="data">
      <caption>Pacientes</caption>
      <table class="table">
        <thead>
            <tr>
                <th scope="col">id</th>
                <th scope="col">Nombre</th>
                <th scope="col">Edad</th>
                <th></th>
            </tr>
        </thead>
        <tbody>
          <tr v-for="(paciente, index) in pacientes" :key="paciente.id">
            <td>{{ paciente.id }}</td>
            <td>
              <span v-if="formActualizar && idActualizar == index">
                <!-- Formulario para actualizar -->
                <input v-model="nombreActualizar" type="text" class="form-control">
              </span>
              <span v-else>
                <!-- Dato nombre -->
                {{ paciente.nombre }}
              </span>
            </td>
            <td>
              <span v-if="formActualizar && idActualizar == index">
                <!-- Formulario para actualizar -->
                <input v-model="edadActualizar" type="text" class="form-control">
              </span>
              <span v-else>
                <!-- Dato edad -->
                {{ paciente.edad }}
              </span>
            </td>
            <td>
              <!-- Botón para guardar la información actualizada -->
              <span v-if="formActualizar && idActualizar == index">
                  <button @click="guardarActualizacion(index)" class="btn btn-success">Guardar</button>
              </span>
              <span v-else>
                  <!-- Botón para mostrar el formulario de actualizar -->
                  <button @click="verFormActualizar(index)" class="btn btn-warning">Actualizar</button>
                  <!-- Botón para borrar -->
                  <button @click="borrarPaciente(index)" class="btn btn-danger">Borrar</button>
              </span>
            </td>
          </tr>
        </tbody>
      </table>
    </section>
  </div>
  ```

<div style="page-break-after: always;"></div>

#### 10.1.2 Parte VUE.js del CRUD

  ```js
<script>
  const app = Vue.createApp({
    data() {
      return {
        nombre: '',            // Input nombre
        edad: '',              // Input edad
        formActualizar: false, // Ver o no ver el formulario de actualizar
        idActualizar: -1,      // Posición de tu lista donde te gustaría actualizar
        nombreActualizar: '',  // Input nombre dentro del formulario de actualizar
        edadActualizar: '',    // Input edad dentro del formulario de actualizar
        pacientes: []          // Lista de pacientes
      };
      },
        methods: {
            crearPaciente() {
                // Añadimos a nuestra lista
                this.pacientes.push({
                    id: +new Date(),
                    nombre: this.nombre,
                    edad: this.edad
                });   
                // Vaciamos el formulario de añadir
                this.nombre = '';
                this.edad = '';
            },
            verFormActualizar(paciente_id) {
            // Antes de mostrar el formulario de actualizar, rellenamos sus campos
                this.idActualizar = paciente_id;
                this.nombreActualizar = this.pacientes[paciente_id].nombre;
                this.edadActualizar = this.pacientes[paciente_id].edad;
                // Mostramos el formulario
                this.formActualizar = true;
            },
            borrarPaciente(paciente_id) {
                // Borramos de la lista
                this.pacientes.splice(paciente_id, 1);
            },
            guardarActualizacion(paciente_id) {
                // Ocultamos nuestro formulario de actualizar
                this.formActualizar = false;
                // Actualizamos los datos
                this.pacientes[paciente_id].nombre = this.nombreActualizar;
                this.pacientes[paciente_id].edad = this.edadActualizar;
            }
        }
    })
    app.mount('#appPacientes');
</script>
```
<div style="page-break-after: always;"></div>

## 11 CRUD paso a paso

### 11.1 Crear (Create)

>Parte HTML

```html
<!-- Formulario para añadir pacientes -->
<section class="form">
    <form action="" class="text-center">
        <input v-model="nombre" @keyup.enter="crearPaciente" type="text" class="form-control" placeholder="Nombre">
        <input v-model="edad" @keyup.enter="crearPaciente" type="number" name="edad" placeholder="Edad" class="form-control">
        <!-- Botón para añadir -->
        <input @click="crearPaciente" type="button" value="Añadir" class="btn btn-success">
    </form>
</section>
```
-------

<br>

>Parte VUE

```js

methods: {
    crearPaciente() {
        // Añadimos a nuestra lista
        this.pacientes.push({
            id: +new Date(),
            nombre: this.nombre,
            edad: this.edad
        });
        // Vaciamos el formulario de añadir
        this.nombre = '';
        this.edad = '';
    }
}
```

------

<div style="page-break-after: always;"></div>

```js
crearPaciente() {
    // Añadimos a nuestra lista
    this.pacientes.push({
        id: +new Date(),
        nombre: this.nombre,
        edad: this.edad
    });
    // Vaciamos el formulario de añadir
    this.nombre = '';
    this.edad = '';
}
```
La función crearPaciente se encarga de agregar un nuevo paciente a la lista pacientes.


```js
this.pacientes.push({
    id: +new Date(),
    nombre: this.nombre,
    edad: this.edad
});
```
Se agrega un nuevo objeto a la lista pacientes con un ID único (generado a partir de la fecha actual), el nombre y la edad proporcionados en el formulario de creación.


```js
this.nombre = '';
this.edad = '';
```
Después de añadir el paciente, se vacían los campos del formulario de creación (nombre y edad) para que estén listos para el siguiente paciente.


```html
<input @click="crearPaciente" type="button" value="Añadir" class="btn btn-success">
```
Cuando el usuario hace clic en este botón, se llama a la función crearPaciente, lo que resulta en la creación de un nuevo paciente y la actualización de la interfaz de usuario.

<div style="page-break-after: always;"></div>

### 11.2 Leer (Read)

```html
<!-- Tabla donde se muestran los datos -->
<section class="data">
    <caption>Pacientes</caption>
    <table class="table">
        <thead>
            <tr>
                <th scope="col">id</th>
                <th scope="col">Nombre</th>
                <th scope="col">Edad</th>
                <th></th>
            </tr>
        </thead>
        <tbody>
            <tr v-for="(paciente, index) in pacientes" :key="paciente.id">
                <!-- Datos de cada paciente -->
                <td>{{ paciente.id }}</td>
                <td>{{ formActualizar && idActualizar == index ? <input v-model="nombreActualizar" type="text" class="form-control"> : paciente.nombre }}</td>
                <td>{{ formActualizar && idActualizar == index ? <input v-model="edadActualizar" type="text" class="form-control"> : paciente.edad }}</td>
                <td>
                    <!-- Botones para actualizar y borrar -->
                    <span v-if="formActualizar && idActualizar == index">
                        <button @click="guardarActualizacion(index)" class="btn btn-success">Guardar</button>
                    </span>
                    <span v-else>
                        <button @click="verFormActualizar(index)" class="btn btn-warning">Actualizar</button>
                        <button @click="borrarPaciente(index)" class="btn btn-danger">Borrar</button>
                    </span>
                </td>
            </tr>
        </tbody>
    </table>
</section>
```
------

<div style="page-break-after: always;"></div>

```html
<tr v-for="(paciente, index) in pacientes" :key="paciente.id">
```
Se utiliza un bucle v-for para iterar sobre la lista de pacientes (pacientes). Cada paciente se representa en una fila de la tabla. El :key asegura que cada fila tenga una clave única basada en el ID del paciente.


```html
<td>{{ paciente.id }}</td>
<td>
    <span v-if="formActualizar && idActualizar == index">
        <!-- Formulario para actualizar -->
        <input v-model="nombreActualizar" type="text" class="form-control">
    </span>
    <span v-else>
        <!-- Dato nombre -->
        {{ paciente.nombre }}
    </span>
</td>
<td>
    <span v-if="formActualizar && idActualizar == index">
        <!-- Formulario para actualizar -->
        <input v-model="edadActualizar" type="text" class="form-control">
    </span>
    <span v-else>
        <!-- Dato edad -->
        {{ paciente.edad }}
    </span>
</td>
```
Se muestran los datos del paciente en cada celda de la fila de la tabla. Se utiliza v-if y v-else para determinar si se debe mostrar el dato estático del paciente o el formulario de actualización.


```html
<button @click="guardarActualizacion(index)" class="btn btn-success">Guardar</button>
<button @click="verFormActualizar(index)" class="btn btn-warning">Actualizar</button>
<button @click="borrarPaciente(index)" class="btn btn-danger">Borrar</button>
```
Se proporcionan botones para actualizar (Actualizar y Guardar) y borrar (Borrar) un paciente. Cada botón está asociado a su respectiva función en Vue.js (guardarActualizacion, verFormActualizar, borrarPaciente).



<div style="page-break-after: always;"></div>

### 11.3 Actualizar (Update)

```js
methods: {
    verFormActualizar(paciente_id) {
        // Antes de mostrar el formulario de actualizar, rellenamos sus campos
        this.idActualizar = paciente_id;
        this.nombreActualizar = this.pacientes[paciente_id].nombre;
        this.edadActualizar = this.pacientes[paciente_id].edad;
        // Mostramos el formulario
        this.formActualizar = true;
    },
    guardarActualizacion(paciente_id) {
        // Ocultamos nuestro formulario de actualizar
        this.formActualizar = false;
        // Actualizamos los datos
        this.pacientes[paciente_id].nombre = this.nombreActualizar;
        this.pacientes[paciente_id].edad = this.edadActualizar;
    }
}
```

-----

<br> 

```js
guardarActualizacion(paciente_id) {
  this.formActualizar = false; // Ocultamos nuestro formulario de actualizar
  this.pacientes[paciente_id].nombre = this.nombreActualizar;// Actualizamos datos
  this.pacientes[paciente_id].edad = this.edadActualizar;
}
```
- La función guardarActualizacion toma un parámetro paciente_id, que es el índice del paciente que se va a actualizar.

```js
this.formActualizar = false;
```
- Se establece formActualizar en false para ocultar el formulario de actualización. Esto sucede después de que el usuario ha hecho clic en el botón "Guardar" y se ha completado la actualización.

<div style="page-break-after: always;"></div>


```js
this.pacientes[paciente_id].nombre = this.nombreActualizar;
this.pacientes[paciente_id].edad = this.edadActualizar;
```
- Se actualizan los datos del paciente en la lista pacientes con la información proporcionada en el formulario de actualización (nombreActualizar y edadActualizar).

```html
<button @click="guardarActualizacion(index)" class="btn btn-success">Guardar</button>
```
- Cuando el usuario hace clic en este botón, se llama a la función guardarActualizacion con el índice correspondiente al paciente en esa fila, y los datos del paciente se actualizan en la lista pacientes.


### 11.4 Borrar (Delete)

```js
methods: {
    borrarPaciente(paciente_id) {
        // Borramos de la lista
        this.pacientes.splice(paciente_id, 1);
    }
}
```

-----

<br>

```js
borrarPaciente(paciente_id) {
    // Borramos de la lista
    this.pacientes.splice(paciente_id, 1);
}
```
- La función **borrarPaciente** toma un parámetro **paciente_id**, que es el índice del paciente que se va a eliminar. 

<br>

```js
this.pacientes.splice(paciente_id, 1);
```
- Utilizando el método **splice** de JavaScript, se elimina un elemento de la lista pacientes en el índice especificado **(paciente_id)**. El segundo argumento (1) indica que **solo** se debe eliminar un elemento en esa posición.

<br>

```html
<button @click="borrarPaciente(index)" class="btn btn-danger">Borrar</button>
```
- Al pulsar el boton se llama a la funcion **borrarPaciente** con el índice correspondiente al paciente en esa fila, y el paciente se elimina de la lista pacientes

<div style="page-break-after: always;"></div>

## 12 ¿Que es vuex?

Vuex es una implementación de la arquitectura de gestión de estado Flux, diseñada específicamente para trabajar con Vue.js. Proporciona un almacén centralizado que contiene todos los estados de la aplicación y reglas para cambiar esos estados de manera predecible. Esto facilita el seguimiento de los cambios de estado y asegura que los componentes de la aplicación siempre tengan acceso actualizado al estado global.

## 12.1 Principales Conceptos en Vuex:

### 12.1.1 Estado (State):

Representa el estado centralizado de la aplicación. Es similar a los datos locales en un componente, pero está disponible globalmente para toda la aplicación.

-------------------------

### 12.1.2  Mutaciones (Mutations):

Son funciones que modifican el estado. Se utilizan para realizar cambios síncronos en el estado. Cada mutación tiene un nombre y un cuerpo que especifica cómo cambiar el estado.

-------------------------

### 12.1.3  Acciones (Actions):

Las acciones contienen la lógica de negocio y llaman a las mutaciones para realizar cambios en el estado. Pueden ser asíncronas y son útiles para realizar operaciones asíncronas como llamadas a API.

-------------------------

### 12.1.4 Getters:

Son funciones que permiten acceder al estado de manera derivada o realizar cálculos basados en el estado actual. Son útiles para obtener vistas específicas del estado sin modificarlo directamente.

-------------------------

### 12.1.5 Módulos:

Vuex permite dividir el almacén en módulos más pequeños, cada uno con su propio estado, mutaciones, acciones y getters. Esto es útil para organizar y modularizar el código en aplicaciones más grandes.
¿Cuándo Deberías Usar Vuex?

-------------------------

## 12.2 Vuex es beneficioso cuando:

1. Tu aplicación tiene un estado complejo y compartido entre varios componentes.
2. Necesitas realizar cambios en el estado de manera predecible y con un flujo de datos unidireccional.
3. La gestión del estado se vuelve difícil de manejar solo con props y eventos entre componentes.

>  Si tu proyecto es más simple, puedes empezar sin Vuex y luego incorporarlo según sea necesario a medida que crece la complejidad de tu aplicación. Sin embargo, Vuex puede ser una herramienta poderosa y eficaz para mantener el estado de tu aplicación en un solo lugar y hacer que el flujo de datos sea más claro y mantenible.




## 13. Vue Router

Vue Router es la biblioteca oficial de enrutamiento para aplicaciones Vue.js. Proporciona una forma de gestionar la navegación en una aplicación de una sola página (SPA), donde los cambios en la URL no provocan recargas de página completas. El navegador solo hace una solicitud al servidor para la carga inicial de la página y cuando la URL cambia (por ejemplo, de https://cochesdelujo.com a https://cochesdelujo.com/mercedes/) depende de Vue determinar qué contenido debe ser mostrado. Con Vue Router, puedes definir rutas y vincularlas a componentes específicos, lo que facilita la creación de aplicaciones con múltiples vistas.

En resumen, Vue Router es una herramienta esencial para crear aplicaciones Vue.js que requieren una navegación fluida entre diferentes vistas sin recargar la página completa.

Principales conceptos y características de Vue Router:

### 13.1 Rutas (Routes)

- Las rutas definen las correspondencias entre las URL y los componentes Vue. Cada ruta puede estar asociada a un componente específico.
  ```javascript
  const routes = [
  { path: '/inicio', component: Inicio },
  { path: '/acerca', component: Acerca },
  ];
  ```

### 13.2 Enrrutamiento Anidado

- Vue Router permite la creación de rutas anidadas, lo que significa que puedes tener componentes dentro de componentes y asociar rutas a cada nivel.
  ```javascript
  const routes = [
  {
    path: '/usuario/:id',
    component: Usuario,
    children: [
      { path: 'perfil', component: Perfil },
      { path: 'configuracion', component: Configuracion }
    ]
  }
  ];
  ```

<div style="page-break-after: always;"></div>


### 13.3 Navegacion Programática

- Puedes navegar entre rutas de forma programática utilizando métodos proporcionados por el enrutador.
  ```javascript
    this.$router.push('/acerca');
  ```

### 13.4 Parámetros de ruta

- Vue Router permite la captura de parámetros dinámicos en las URL, lo que facilita la creación de rutas dinámicas.
  
```javascript
const routes = [
  { path: '/usuario/:id', component: Usuario }
];
```

### 13.5 Transiciones de Vista

- Puedes aplicar transiciones y animaciones a las vistas al cambiar entre rutas.

### 13.6 Guardias de Navegación

- Las guardias de navegación te permiten controlar la navegación antes de que se active una ruta, útil para la autenticación, autorización y validación de datos.

  ```javascript
  const router = new VueRouter({
    routes,
    beforeEnter(to, from, next) {
      // Lógica de guardia
    }
  });
  ```

<div style="page-break-after: always;"></div>


### 13.7 Modo de Historial

- Puedes elegir entre el modo de historial HTML5 (history) o el modo de hash (hash) para manejar las URL.
  
  ```javascript
  const router = new VueRouter({
  mode: 'history',
  routes
  });
  ```

### 13.8 Lazy Loading de COmponentes

- Vue Router es compatible con la carga perezosa de componentes, lo que significa que los componentes se cargan solo cuando se necesitan, mejorando los tiempos de carga inicial.

  ```javascript
  const routes = [
    { path: '/inicio', component: () => import('./Inicio.vue') }
  ];
  ```


<div style="page-break-after: always;"></div>

## 14. Mantenimiento y Escalabilidad

1. **Estructura y Organización del Proyecto:**<br>
Módulos y Componentes Reutilizables: Divide tu aplicación en módulos y componentes reutilizables para facilitar el mantenimiento y la comprensión del código.
<br><br>
Estructura del Proyecto: Organiza tu código de manera lógica, separando componentes, estilos y lógica de negocio.

-------------------------

2. **Gestión del Estado con Vuex:**<br>
Vuex para Estado Global: Usa Vuex para gestionar el estado global de tu aplicación. Esto facilita la centralización de la lógica de estado y simplifica el seguimiento de cambios.
<br><br>
Módulos en Vuex: Divide el estado de Vuex en módulos para escalabilidad. Cada módulo puede manejar su propio estado, mutaciones, acciones y getters.

-------------------------

3. **Optimización del Rendimiento:**<br>
Directivas v-if vs v-show: Comprende cuándo usar v-if y v-show para optimizar el rendimiento según la necesidad de renderización condicional.
<br><br>
Optimización de Renderización: Utiliza herramientas como shouldComponentUpdate (en componentes de clase) o memo (en componentes funcionales) para evitar renderizaciones innecesarias.

-------------------------

4. **Manejo de Rutas con Vue Router:**<br>
Lazy Loading de Rutas: Implementa la carga perezosa de componentes para evitar que la aplicación cargue todo el código de una sola vez, mejorando los tiempos de carga inicial.
<br><br>
Rutas Anidadas: Estructura las rutas de manera jerárquica, especialmente si tu aplicación crece en complejidad.

-------------------------

5. **Pruebas Unitarias y de Integración:**<br>
Pruebas Automatizadas: Implementa pruebas unitarias y de integración para asegurar la estabilidad de tu aplicación durante el desarrollo y las actualizaciones.
<br><br>
Herramientas de Pruebas: Utiliza bibliotecas como Jest y herramientas como Vue Test Utils para facilitar la escritura y ejecución de pruebas.

-------------------------

<div style="page-break-after: always;"></div>

6. **Despliegue y Configuración para Producción:**<br>
Optimización de Código: Minimiza y ofusca el código para reducir el tamaño de los archivos y mejorar los tiempos de carga.
<br><br>
CDN y Caché: Utiliza CDNs para entregar recursos estáticos y configura estrategias de caché para optimizar la velocidad de carga de la aplicación.

-------------------------

7. **Escalabilidad Horizontal y Vertical:**<br>
Escalabilidad Vertical: Aumenta los recursos (CPU, RAM) en una única máquina para manejar cargas más grandes.
<br><br>
Escalabilidad Horizontal: Distribuye la carga distribuyendo la aplicación en varias máquinas. Utiliza servicios de equilibrio de carga y gestión de clústeres.

-------------------------

8. **Seguridad:**<br>
Prácticas de Seguridad: Implementa buenas prácticas de seguridad, como validación de entrada, prevención de ataques de inyección, y aseguramiento de la comunicación.
<br><br>
Actualizaciones y Parches: Mantén tu aplicación y las dependencias actualizadas para protegerte contra vulnerabilidades conocidas.

-------------------------

9. **Documentación y Comentarios:**<br>
Documentación Clara: Documenta tu código y la estructura de tu aplicación para facilitar la comprensión y el mantenimiento por parte de otros desarrolladores.
<br><br>
Comentarios Significativos: Utiliza comentarios significativos para explicar decisiones arquitectónicas o soluciones específicas.

-------------------------

10. **Monitoreo y Análisis:**<br>
Monitoreo de Rendimiento: Utiliza herramientas de monitoreo para rastrear el rendimiento de la aplicación y solucionar problemas rápidamente.
<br><br>
Análisis de Errores: Implementa servicios de seguimiento de errores para identificar y solucionar problemas en tiempo real.

-------------------------
<div style="page-break-after: always;"></div>

## 15. Fuentes
[Índice](#tabla-de-contenidos)
  - **ChatGPT:** https://chat.openai.com
  - **Aria:** https://www.opera.com/es-419/features/aria 
  - **W3schools:** https://www.w3schools.com/vue/index.php
  - **vuejs:** https://es.vuejs.org
  - **ProgramadorWebValencia** https://programadorwebvalencia.com/vuejs-crud-sencillo/
  - **Neunapp:** https://www.youtube.com/@Neunapp
  - **Medium:** https://medium.com/@khriztianmoreno/vue-router-66a2c5f4c71e