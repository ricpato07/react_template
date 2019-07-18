# react_template

**Plugins para React en VSC**

ESLint - Dirk Baeumer

Bracket Pair Colorizer - CoenraadS

Reactjs code snippets - charalampos karypidis

ES7 React/Redux/GraphQL/React-Native snippets - dsznajder

generate-react-component - joshjg


**Javascript:**

Spread operator

```
arreglo1 = ['hola','como', 'estas']
arreglo2 = ['hola','como', 'estas']

juntarArreglos = [...arreglo1,...arreglo2]
copiaArreglo1 = [...arreglo1]

```

Destructuring 

```
const aprendiendoJS = {
    version: { nueva: 'ES6',
               anterior: 'ES5'
              },
     frameworks: ['Angular', 'Laravel', 'Spring']         
  }
  
  let {version, frameworks} = aprendiendoJS;
  
```
Object Literal Enhacement

```
const banda = 'Metallica';
const genero = 'Heavy Metal'
const canciones = ['Sick & destroy', 'Unforgiven'];

const metallica = {banda, genero, canciones};

```

Object Keys (regresa las llaves de un objeto)

```
const persona = {
     nombe: 'Juan',
     profesion: 'programador',
     edad : 30
     }
     
 Objects.keys(persona);    
     
```

filter , find

```
const personas = [
     {nombre: "Juan", edad: 23, aprendiendo: "Javascript"},
     {nombre: "Pablo", edad: 18, aprendiendo: "PHP"},
     {nombre: "Alejandra", edad: 20, aprendiendo: "Adobe"},
     {nombre: "Karen", edad: 38, aprendiendo: "Python"},
     {nombre: "Miguel", edad: 35, aprendiendo: "React"}
]

//regresa arreglo con persona mayores a 28 años
const mayores = personas.filter(persona =>{
 return persona.edad > 28;
}) 

//retorno objeto de Alejandra
const alejandra = personas.find(persona =>{
  return persona.nombre === 'Alejandra';
})

//resgresar la suma de las edades
let total = personas.reduce((edadtotal,persona)=>{
  return edadTotal + persona.edad;
}, 0)
     
```

Promises
```
const aplicarDescuento = new Promise((resolve, reject)=>{
  setTimeout(()=>{
  let descuento = true;
   if(descuento){
     resolve("Descuento aplicado");
   }else{
   reject("No se pudo aplicar el descuento");
   }
  },3000);
})

aplicarDescuento.then(resultado =>{
  console.log(resultado);
})
```

----------------------------------------------------------
Crear un nuevo proyecto de react
----------------------------------------------------------

Crear un nuevo proyecto
npx create-react-app my-app

Instalar librerias
npm install

Corre servidor
npm start

----------------------------------------------------------
Servidor local
----------------------------------------------------------
Instalar servidor local
npm install -g serve

Correr servidor local
serve -s build
----------------------------------------------------------

----------------------------------------------------------
REDUX
----------------------------------------------------------

Instalar Redux
npm install redux --save 

Instalar Redux-React 
npm install react-redux --save

Instalar Redux-thunk
npm install redux-thunk --save

Instalar Reduc-saga
npm install redux-saga --save

----------------------------------------------------------

----------------------------------------------------------
BULMA
----------------------------------------------------------

Instalar Bulma
npm install bulma --save --save-exact

----------------------------------------------------------

----------------------------------------------------------
PROP-TYPES
----------------------------------------------------------
Instalar prop-types
npm install --save prop-types

----------------------------------------------------------

----------------------------------------------------------
REACT-ROUTER
----------------------------------------------------------
npm install react-router-dom --save

----------------------------------------------------------

Ruta carpeta para colocar el node-sass
C:\Users\45042195\AppData\Roaming\npm-cache\node-sass

Instalar WebPack
npm install webpack --save-dev

Instalar el cliente de WebPack
npm install webpack-cli --save-dev

Herramientas necesarias para desarrollar:

Cliente y herramientas para el desarrollo
Creación de componentes básicos
Creación de templates
Links y url para mostrar deferentes páginas
Libreria para realizar peticiones
Uso de clases o interfaces para manejo de datos
Uso de constantes
Uso de componentes para el formulario
Validaciones del formulario
Creación de ventanas modal
Manejo de variables (Enviroment variables) para diferentes ambientes
Guardado de información en sesión
Compilado para producción


Create React App 
Crea una aplicación en React
https://facebook.github.io/create-react-app/docs/getting-started

WebPack
Agrupar proyecto, crea compilados
https://webpack.js.org/guides/getting-started/

Babel
Hace compatible el código credo en jsx a un javascript simple
https://babeljs.io/docs/en/

Redux
Herramienta para manejar eventos en la aplicación
https://redux.js.org/introduction/getting-started
Videos de Redux
https://egghead.io/lessons/react-redux-the-single-immutable-state-tree
Guia completa para Redux desde 0
https://www.valentinog.com/blog/redux/

Mobx
Manejo de los observables, similar a redux
https://mobx.js.org/index.html

Material UI
Componentes predefinidos con estilos
https://material-ui.com/getting-started/installation/


React Final Form
Formularios en React
https://github.com/final-form/react-final-form#-react-final-form

Redux-form
Otro manejo de formularios
https://github.com/erikras/redux-form

The complete guide to Forms in React
Validacion de campos desde cero
https://medium.com/@agoiabeladeyemi/the-complete-guide-to-forms-in-react-d2ba93f32825


Fetching data from an api using React/Redux
Realizar peticiones con Redux
https://dev.to/markusclaus/fetching-data-from-an-api-using-reactredux-55ao
https://stackoverflow.com/questions/38728884/how-to-properly-make-rest-calls-from-reactjs-redux-application


React Router
Enlaces entre páginas
https://reacttraining.com/react-router/web/example/sidebar


Browserify
Importa la librerias utilizadas en Node
http://browserify.org/#more


SystemJS
Cargador de módulos de Javascript
https://github.com/systemjs/systemjs

React for Angular Developers
Componentes de React comparándolos con AngularJS
https://www.sitepoint.com/react-for-angular-developers/


Interfaces implementadas en React
https://stackoverflow.com/questions/36745013/interface-states-and-props-in-typescript-react


User variables en session
https://stackoverflow.com/questions/42420531/what-is-the-best-way-to-manage-a-users-session-in-react

Compatibilidad de React en Explorer
https://github.com/facebook/create-react-app/blob/master/packages/react-app-polyfill/README.md

Compilando proyecto con Webpack
https://medium.com/@sergiodxa/compilando-el-frontend-con-webpack-d251f7a632ec

my-app
+-- build
+-- node_modules
+-- public
¦   +-- favicon.ico
¦   +-- index.html
¦   +-- manifest.json
+-- 
src
¦   +-- assets
¦   ¦   +--images
¦   ¦      +-- logo.svg
¦   +-- components
¦   ¦   +-- app
¦   ¦       +-- app.css
¦   ¦       +-- app.js
¦   ¦       +-- app.test.js
¦   +-- utils
¦   +--
 index.css
¦   +-- index.js
¦   +-- service-worker.js+-- .gitignore
+-- package.json
+-- README.md

