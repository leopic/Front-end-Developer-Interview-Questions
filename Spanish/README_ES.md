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
	* De ser asi, cuales librerias has usado (Mustache.js, Handlebars etc.) 
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
* Describe a strategy for memoization (avoiding calculation repetition) in JavaScript. 
* Why is it called a Ternary statement, what does the word "Ternary" indicate? 
* Que es el `arity` para una funcion?

## JS-Code Examples:

```javascript
~~3.14
```
Question: What value is returned from the above statement? 
**Answer: 3** 

```javascript
"i'm a lasagna hog".split("").reverse().join("");
```
Question: What value is returned from the above statement? 
**Answer: "goh angasal a m'i"** 

```javascript
( window.foo || ( window.foo = "bar" ) );
```
Question: What is the value of window.foo? 
**Answer: "bar"** 
only if window.foo was falsey otherwise it will retain its value.

```javascript
var foo = "Hello"; (function() { var bar = " World"; alert(foo + bar); })(); alert(foo + bar);
```
Question: What is the outcome of the two alerts above? 
**Answer: "Hello World" & ReferenceError: bar is not defined** 

```javascript
var foo = [];
foo.push(1);
foo.push(2);
```
Question: What is the value of foo.length? 
**Answer: `2`

```javascript
var foo = {};
foo.bar = 'hello';
```
Question: What is the value of foo.length? 
**Answer: `undefined`


## jQuery-Specific Questions:

* Explain "chaining". 
* Explain "deferreds".
* What are som jQuery specific optimizations you can implement?
* What does `.end()` do? 
* How, and why, would you namespace a bound event handler? 
* Name 4 different values you can pass to the jQuery method?
	* Selector (string), HTML (string), Callback (function), HTMLElement, object, array, element array, jQuery Object etc.
* What is the effects (or fx) queue? 
* What is the difference between `.get()`, `[]`, and `.eq()`? 
* What is the difference between `.bind()`, `.live()`, and `.delegate()`? 
* What is the difference between `$` and `$.fn`? Or just what is `$.fn`.
* Optimize this selector: 
```javascript
$(".foo div#bar:eq(0)")
```

## CSS-Specific Questions:

* Describe what a "reset" CSS file does and how it's useful. 
* Describe Floats and how they work. 
* What are the various clearing techniques and which is appropriate for what context? 
* Explain CSS sprites, and how you would implement them on a page or site. 
* What are your favourite image replacement techniques and which do you use when? 
* CSS property hacks, conditionally included .css files, or... something else? 
* How do you serve your pages for feature-constrained browsers? 
	* What techniques/processes do you use?  
* What are the different ways to visually hide content (and make it available only for screen readers)? 
* Have you ever used a grid system, and if so, what do you prefer? 
* Have you used or implemented media queries or mobile specific layouts/CSS? 
* Any familiarity with styling SVG? 
* How do you optimize your webpages for print? 
* What are some of the "gotchas" for writing efficient CSS? 
* Do you use CSS preprocessors? (SASS, Compass, Stylus, LESS) 
	* If so, describe what you like and dislike about the CSS preprocessors you have used. 
* How would you implement a web design comp that uses non-standard fonts? 
	* Webfonts (font services like: Goodle Webfonts, Typekit etc.)
* Explain how a browser determines what elements match a CSS selector?  

## Optional fun Questions:

* What's the coolest thing you've ever coded, what are you most proud of?
* Do you know the HTML5 gang sign? 
* Are you now, or have you ever been, on a boat. 
* What are your favorite parts about the developer tools you use?
* Do you have any pet projects? What kind? 
* Explain the significance of "cornify". 
* On a piece of paper, write down the letters A B C D E vertically. Now put these in descending order without writing one line of code. 
	* Wait and see if they turn the paper upside down
* Pirate or Ninja? 
	* Bonus if it's a combo and a good reason was given (+2 for zombie monkey pirate ninjas) 
* If not Web Development, what would you be doing? 
* Where in the world is Carmen Sandiego?
	* Hint: their answer is always wrong 
* What's your favorite feature of Internet Explorer?
* Complete this sentence: Brendan Eich and Doug Crockford are the __________ of javascript.
* jQuery: a great library or the greatest library? Discuss.

