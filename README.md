1. ¿Qué es la lógica en el contexto de la programación? Y explicar por qué es importante 
en el desarrollo web Frontend.

R//: Es la capacidad de darle solucion a los algoritmos de programacion, es importante para tener buen flujo de codigo y buena interaccion con el usuario.

2. Definir el concepto de “algoritmo” y proporcionar un ejemplo sencillo de un algoritmo 
relacionado con la lógica de programación.

R//: Es la manera de darle orden a una solucion del problema planteado.

**EJEMPLO** : si la multiplicacion de los valores es 6 que me imprima es par de lo contrario es impar.

3. ¿Qué son estructuras de control en la programación?, ¿Cuáles son los tipos de 
estructuras de control y las estructuras más comunes de cada tipo?, Describir al menos 
dos tipos de estructura de control, explicar por qué son importantes y proporcionar 
ejemplos de cada uno de cómo se utilizan en el desarrollo web Frontend.

R//: son las reglas que permiten el flujo o modificacion de la ejecucion, los tipos de estructuras de control son secuenciales, selectivas, iterativas

**Secuenciales**:
las secuenciales son la que nos permiten que el codigo se ejecute en el orden que fueron escritas.
**EJEMPLO**: puede ser la estructura de una pagina
**Selectivas(o condicionales)**:
son las estructuras que nos permiten crear una condicion de que nos evalue el valor para poder dar la instructucion de la siguiente ejecucion.
**EJEMPLO**: if let = 4  true else=false 
**Iteracion(bucles)**:
son las estructuras que nos permiten ejecutar ciertas lineas varias veces repetidas.

4. Describir cómo se declaraban variables y constantes en JavaScript antes de la 
introducción de ECMAScript 6 (ES6). Explicar cómo ES6 mejoró la declaración de 
variables y constantes, y mencionar los problemas que esta mejora resuelve en el 
desarrollo web Frontend.

R//: 
Antes de (ES6) las variables se definian con: *var*;
(ES6) mejoro mas que todo ala hora de poder usar buqles por que la palabra var lo que hacia era crear una variable "global", encambio let es una variable que puede tener cambios y const es un valor fijo.

5. ¿Cómo se declaran las funciones en JavaScript y cuál es la diferencia entre una 
declaración de función, una expresión de función y una función de flecha (arrow 
function)? Proporcionar ejemplos de cada una.

R//: 
 **Declaracion de funcion**
function sumar(a, b) {
    return a + b;
}
*diferencia*: Se puede usar antes de la declaración

**Expresion de funcion**
const multiplicar = function(a, b) {
    return a * b;
};
*diferencia*: No debe de ser declarada antes de usarse

**Funcion de flecha**
const dividir = (a, b) => {
    return a / b;
};
*diferencia*: no debe de ser declarada antes de usarse.

6. ¿Por qué es necesario el uso de funciones en el desarrollo web Frontend? Enumerar al 
menos tres razones fundamentales y proporcionar ejemplos de situaciones en las que 
las funciones son esenciales. Además, mencionar la ventaja de las funciones flecha en 
el contexto de estas razones.

R//: 
1 Una de las razones fundamentales es la reutilizacion de codigo por ejemplo ala hora de validar los datos que ingresan a un formulario esa funcionalidad la podemos reutilizar en varios formularios.

2  la optimizacion de codigo  por ejemplo poder hacer lo mismo con menos lineas de codigo.

3   El manejo de eventos con interaccion de apis ejemplo cuando tenemos que hacer peticiones http.

7. ¿Cuál es la diferencia entre parámetro y argumento?

R//: 
La diferencia es que *parametros* son variables que se definen en una funcion y *argumentos* son valores reales que se le pasan ala funcion.

8. Definir el concepto de Callback y proporcionar un ejemplo práctico.

R//:
Es una funcion que se le pasa como argumento a otra funcion y su ejecucion se efectua con  un evento.

9. ¿Qué es el hoisting en JavaScript y cómo afecta a las variables y funciones? 
Proporcionar ejemplos de hoisting en declaraciones de variables y funciones.

R//:
Es cuando una funcion se llama antes de ser declarada,   y en la manera que afecta es por que podemos tener resultados inesperados al estar llamando la funcion sin ser declarada.

**Ejemplos**

console.log(y); // undefined
let y = 18;
console.log(y); // 18



hello(); // "Hola, mundo"

function hello() {
console.log("Hola, mundo");
}


bye(); // TypeError

let bye = function() {
console.log("adios");
};


10. Definir brevemente el concepto de objeto en JavaScript y cuál es la visión general sobre 
este concepto. Indicar, también cómo se declaran estas estructuras de datos.

R//: 
Es una estructura de datos que nos permite almacenar informacion de una persona u objeto de la vida cotidiana


**Declaracion de un objeto**
let persona = {
    nombre: "Luis",
    edad: 25,
    genero: "Masculino"
    saludar: function() {
    console.log("Hola, soy " + this.nombre + ".");
    }
}

11. ¿Qué son propiedades?, y ¿Cuál es la diferencia entre una propiedad y un método en 
un objeto?

R//: 
Las propiedades son los datos del objeto que teniene cierta informacion de el, y la diferencia es que un metodo es una propiedad pero el valor es una funcion .

12. Explicar las dos formas de acceder a una propiedad de objetos e indicar las situaciones 
en que conviene usar una manera sobre la otra.

R//: 
1.1. objeto.propiedad
la notacion de punto es mejor usarla cuando sabemos de antemano el resultado.

1.2. objeto["propiedad"]
la notacion de corchetes es mejor usarla cuando necesitamos acceder a una propiedad de manera dinamica o cuando es definida en variables o expresiones.


13. ¿Existe alguna forma de recorrer las propiedades de un objeto? En caso negativo, 
explicar por qué no es posible y en caso positivo proporcionar un ejemplo. Mencionar 
una situación en la cual sea muy útil recorrer las propiedades de un objeto.

R//: 
Si existen varias formas de recorrer un objeto la mas usual es con un buqle, las situaciones donde es util recorrer las propiedades de un objeto es cuando trabajamos con datos dinamicos y obtemos informacion de una API.

**Ejemplo**

function mostrarPropiedadesEnInterfaz(objeto) {
  for (let propiedad in objeto) {
    if (objeto.hasOwnProperty(propiedad)) {
      var elemento = document.createElement("p");
      elemento.textContent = propiedad + ": " + objeto[propiedad];
      document.body.appendChild(elemento);
    }
  }
}

var datosUsuario = {
  nombre: "Juan",
  edad: 30,
  correo: "juan@example.com"
};

mostrarPropiedadesEnInterfaz(datosUsuario);

14. ¿Por qué son útiles los objetos en la programación web y qué tipos de datos pueden 
almacenar?

R//: 
Son utiles por la capacidad de organizar y estructurar datos de manera mas eficiente, y por la flexibilidad del manejo de los datos.

15. ¿Qué es un array en JavaScript y por qué son esenciales?

R//: 
Un array es una lista que nos permite almacenar valores u objetos y son esenciales por que nos permiten tener un flujo de trabajo mas simple y optimizado.

16. ¿Cómo acceder a un elemento dentro de un array? Explicar con un ejemplo.

R//: 
**Ejemplo**

let nombres = ["Ana", "Juan", "María", "Carlos"];

let primerNombre = nombres[0];
console.log(primerNombre); // Ana

var tercerNombre = nombres[2];
console.log(tercerNombre); // Maria

17. Mencionar al menos tres funciones de arrays y describir su utilidad en la programación 
web.

R//: 
**.find**: Nos devulve el primer elemento que tengas las condiciones requeridas.
**.map**: Nos transforma un array en otro con diferentes condiciones.
**.filter**: Nos devulve otro array pero con las condiones de la necesidad de informacion que tenemos.

18. Proporcionar un ejemplo de cómo se utiliza una función de array para transformar y 
filtrar datos en un array.

R//: 
const numeros = [5, 8, 12, 3, 15, 7, 9];

*const numerosDuplicados = numeros.map(numero => numero * 2);*

*const numerosFiltrados = numerosDuplicados.filter(numero => numero >= 10);*

