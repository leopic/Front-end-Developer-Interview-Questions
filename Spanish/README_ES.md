#GUIA DE PREGUNTAS PARA ENTREVISTAS DE TRABAJO

@version 1.0
 
##Contribuyentes

@bentruyman (http://bentruyman.com/), @roger_raymond (http://twitter.com/iansym), @ajpiano (http://ajpiano.com/), @paul_irish (http://paulirish.com/), @SlexAxton (http://alexsexton.com/), @boazsender (http://boazsender.com/), @miketaylr (http://miketaylr.com/), @vladikoff (http://vladfilippov.com/), @gf3 (http://gf3.ca/), @jon_neal (http://twitter.com/jon_neal), @wookiehangover (http://wookiehangover.com/) and @darcy_clarke (http://darcyclarke.me)

## Preguntas Generales:

* Tenes cuenta en Twitter? 
	* De tenerla, a quien seguis en Twitter?
* Tenes cuenta en Github?
	* De tenerla, podes mencionar algunos repositorios que seguis?
* Que blogs seguis?
* Cuales sistema de control de versiones has usado (Subversion, Git, entre otros)?
* Cual es tu ambiente de desarollo favorito (Sistema Operativo, Editor de Texto, Navegadores, Herramientas, entre otras)?
* Podes describir el proceso que seguis cuando creas una pagina web?
* Podes describir la diferencia entre 'Progressive Enhancement' y 'Graceful Degradation'?
	* Puntos extra si describis deteccion de capacidades
* Explica que significa "HTML Semantico"
* Cual es tu navegador primario y cuales herramientas de desarrollo usas?
* Como optimizas los recursos de un website?
	* Se busca una serie de soluciones tales como:
		* Concatenacion de archivos
		* Compresion (minificacion) de archivos
		* Utilizar un CDN
		* Caching
		* Entre otros
* Porque es mejor utilizar varios dominios para distribuir los recursos de una pagina web?
	* Cuantos recursos se pueden descargar simultaneamente de un mismo dominio?
* Menciona tres formas para disminuir el tiempo de carga de una pagina (tiempo real o percibido).
* Imagina que iniciaste en un proyecto, pero los desarrolladores usan tabs y vos espacios, que haces?
	* Sugerir que el proyecto utilice algo como EditorConfig (http://editorconfig.org)
	* Mantener la convencion y utilizar tabs.
	* `utilizar el comando :retab!`
* Escribi un pagina con una galeria sencilla
	* Puntos extra si no utiliza Javascript
* Que herramientas usas para probar el performance de tu codigo?
	* JSPerf (http://jsperf.com/)
	* Dromaeo (http://dromaeo.com/) 
	* Entre otras
* Si podes elegir una tecnologia para dominar este anyo, cual seria?
* Explica la importancia de estandares y los grupos que los definen.

## Preguntas especificas de HTML:

* Que funcion cumple el `doctype` y cuantos podes nombrar?
* Cual es la diferencia entre el modo convencional y el quirks mode?
* Cuales son las limitaciones al utilizar paginas XHTML?
	* Hay algun problema al servir las paginas usando: `application/xhtml+xml`?  
* Como programarias una pagina con contenido en varios lenguajes?
	* Que consideraciones se deben tener cuenta cuando se disenyan o desarrollan sitios multi-lenguajes?
* Podes usar sintaxis de XHTML en HTML5?
* Como usas XML en HTML5?
* Para que se utilizan los atributos `data-`?
* Cuales son los modelos de contenido usados en HTML4, podes comprarlos a los de HTML5? 
* Considera HTML5 como una plataforma web abierta, cuales son las piezas del lego que constituyen HTML5?
* Describi la diferencia entre cookies, sessionStorage y localStorage.

## Preguntas especificas de Javascript:

* Que librerias de Javascript has usado?
* En que se diferencia Javascript de Java?
* Que es un `hashtable`?
* Cual es la diferencia entre variables `undefined` y variables `undeclared`? 
* Que es un closure y cuando, o porque, usarias uno?
* What is a closure, and how/why would you use one? 
	* Cual es tu patron favorito para crearlos? argyle (Solo aplica a las IIFEs)
* Podes hablar de un uso tipico para una funcion anonima?
* Podes explicar el patron modular en Javascript y cuando lo usarias?
	* Puntos extra por mencionar un namespace no contaminado.
	* Que pasa si tus modulos no tienen un namespace?
* Como organizas tu codigo, patron modular, herencia clasica?
* Cual es la diferencia entre objetos huesped (host objects) y objetos nativos?
* Cual es la diferencia entre:
```javascript
function Person(){} var person = Person() var person = new Person()
```
* Cual es la diferencia entre `.call` y `.apply`? 
* Podes explicar el uso de `Function.prototype.bind`? 
* Cuando optimizas tu codigo?
* Podes explicar como funciona la herencia en Javascript?
* Cuando usarias `document.write()`?
	* La mayoria de anuncios de vendors todavia utilizan esta tecnica, aunque no esta recomendad.
* Cual es la diferencia entre deteccion de capacidades, inferencia de capacidades y usar el string del user agent.
* Explique AJAX con tanto detalle como sea posible.
* Explique como funciona JSONP (y como es distinto a AJAX).
* Has utilizado alguna vez templates en Javascript?
	* De ser asi, cuales librerias has usado (Mustache.js, Handlebars, entre otros) 
* Podes explicar en que consiste el "hoisting"?
* Sabes que es el FOUC? Y como evitarlo?
* Podes hablar sobre event bubbling. 
* Cual es la diferencia entre un 'atributo' y una 'propiedad'?
* Porque es una mala idea extender objetos nativos de Javascript?
* Porque es una buena idea extender objetos nativos de Javascript?
* Cual es la diferencia entre el evento document load y document ready?
* Cual es la diferencia entre `==` y `===`? 
* Si tenes que obtener un parametro del URL, como lo harias? 
* Explica la politica de mismo origen (same-origin policy) y sus repercusiones en Javascript.
* Explica event delegation. 
* Podes describir los patrones de herencia en Javascript?
* Arregla este codigo:
```javascript
[1,2,3,4,5].duplicator(); // [1,2,3,4,5,1,2,3,4,5]
```
* Podes describir una estrategia para memoizacion ('memoization', evitar repetir calculos) en Javascript?
* Porque reciben el nombre de sentencias ternarias, que significa la palabra 'Ternaria'?  
* Que es el `arity` para una funcion?

## Ejemplos de codigo de Javascript:

```javascript
~~3.14
```
Pregunta: Cual es el retorno de la sentencia anterior?
**Respuesta: 3** 

```javascript
"i'm a lasagna hog".split("").reverse().join("");
```
Pregunta: Cual es el retorno de la sentencia anterior?
**Respuesta: "goh angasal a m'i"** 

```javascript
( window.foo || ( window.foo = "bar" ) );
```
Preguntan: Cual es el valor de window.foo?
**Respuesta: "bar"** 
Unicamente si window.foo tenia un valor falsey, de cualquier otra forma retendra su valor.

```javascript
var foo = "Hello"; (function() { var bar = " World"; alert(foo + bar); })(); alert(foo + bar);
```
Pregunta: Cual es el resultado de los dos alerts anteriores?
**Respuesta: "Hello World" y ReferenceError: bar is not defined** 

```javascript
var foo = [];
foo.push(1);
foo.push(2);
```
Pregunta: Cual es el valor de foo.length? 
**Respuesta: `2`

```javascript
var foo = {};
foo.bar = 'hello';
```
Pregunta: Cual es el valor de foo.length? 
**Respuesta: `undefined`


## Preguntas especificas de jQuery:

* Explica el "encadenamiento" (chaining).
* Explica las "diferidas" (deferreds).
* Cuales son algunas optimizaciones que se pueden implementar usando jQuery?
* Que funcion cumple el metodo `.end()`? 
* Como y porque, aplicaria namespacing a un event handler?
* Nombre cuatro diferentes valores que se pueden pasar por parametro al metodo jQuery.
	* Un selector (string), HTML (string), Callback (function), HTMLElement, objeto, arreglo, arreglo de elementos, objeto jQuery, entre otros.
* Que es la cola de efectos (fx queue)?
* Cual es la diferencia entre `.get()`, `[]` y `.eq()`? 
* Cual es la diferencia entre `.bind()`, `.live()` y `.delegate()`? 
* Cual es la diferencia entre `$` y `$.fn`? O simplemente, que es `$.fn`?
* Optimize este selector:
```javascript
$(".foo div#bar:eq(0)")
```

## Preguntas espeficicas de CSS:

* Describa que es un "reset" y porque es util?
* Describa los "Floats" y como funcionan.
* Cuales son los metodos para limpiar (clear) floats y cual es apropiado para cual contexto?
* Explica que son los sprites en CSS y como los implementarias en una pagina.
* Cual es tu tecnica favorita para reemplazar imagenes y cuando usas cada una?
* CSS Hacks, archivos incluidos con etiquetas condicionales o algun otro metodo?
* Cual es tu enfoque al desarrollar paginas que dan soporte a navegadores con limitadas capacidades?
	* Que tecnicas o procesos usas?
* Cuales son las distintas formas para esconder contenido, pero mantenerlo disponible unicamente para screen readers?
* Has usado algun sistema de cuadriculas (grids) y cual preferis?
* Has usado o implementado media queres o reglas especifico para dispositivos mobiles?
* Tenes familiaridad con darle estilos a SVGs?
* Como optimizas tus paginas para impresion?
* Cuales son algunos de los "trampas" al escribir CSS eficiente?
* Has usado algun preprocesador para CSS (SASS, Compass, Stylus, LESS)? 
	* De ser asi, podes mencionar que te gusta y que no de los que has usado?
* Como implementarias un disenyo que usa fuentes que no son web-safe?
	* Webfonts (usando servicios para fuentes como Goodle Webfonts, Typekit, entre otros)
* Podes explicar como determina un navegador cuales elementos coinciden con un selector de CSS?

## Preguntas opcionales y divertidas:

* Cual es la cosa mas cool que has programado y que es lo que mas te enorgullece?
* Sabes cual es la senya pandillera (gang sign) para HTML5?
* Estas ahora o has estado alguna vez en un bote?
* Cuales son tus partes favoritas de las herramientas de desarrollo que usas?
* Tenes algun proyecto personal? De que tipo?
* Explica el significado de "cursificar" (cornify).
* Toma un papel y escribi las letras A B C D E verticalmente, ahora ponelas en order descendiente sin escribir una sola linea de codigo.
	* Espera a ver si giran el papel.
* Pirata o Ninja?
	* Puntos extra si es una combinacion y dio una buena razon, dos puntos extra por monos zombies piratas ninjas.
* Si no estuvieras en Desarollo Web, en que estarias trabajando?
* Donde en el mundo esta Carmen Sandiego?
	* Consejo: no hay respuesta correcta.
* Cual es tu funcionalidad favorita de Internet Explorer?
* Completa esta oracion: Brendan Eich y Doug Crockford son los __________ del Javascript.
* jQuery: una buena libreria o la mejor libreria? Explica porque.

