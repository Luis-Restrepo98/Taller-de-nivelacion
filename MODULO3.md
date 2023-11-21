***MÓDULO SOBRE DOM E INTERACCIÓN CON EL DOM***

1. ¿Qué es el DOM (Modelo de Objeto de Documento) en el contexto de la programación 
web?

R//:
Es la interfaz que representa la estructura de un documento html o xml es esencial para interactuar con el html en el script.

2. ¿Cuál es la diferencia entre el DOM y el HTML en una página web?

R//:
la diferencia es que el html es especificamente para trabajar en la estructura de la pagina y el DOM trabaja con los elementos del html pero en el script.

3. ¿Porqué es importante entender y manipular el DOM en el desarrollo web Frontend?

R//:
Por el buen manejo del codigo y poder hacer que las interfaces sean de mas amaño para los usuarios.

4. ¿Qué son los eventos del DOM y cuál es su función en una página web?

R//:
Son sucesos o acciones efectuadas por el usuario y son diseñadas en el script como los eventos de click.

5. Proporcionar ejemplos de eventos prácticos y comunes, como “click”, “submit” y “load o 
DOMContentLoad”.

R//:
**Ejemplos**:
1. 
function handleClick() {
    alert("¡Haz hecho clic!");
}

<button onclick="handleClick()">Haz clic aquí</button>

2. 
function handleSubmit(event) {
    event.preventDefault();
    alert("Formulario enviado");
}

<form onsubmit="handleSubmit(event)">
    <input type="submit" value="Enviar Formulario">
</form>

3. 
document.addEventListener("DOMContentLoaded", function() {
    alert("DOM completamente cargado");
});

6. ¿Por qué es importante manejar eventos en la interacción usuario-web y cómo se 
añaden controladores de eventos a los elementos del DOM?

R//:
Es importante por que permite que las paginas sean interactivas y respondan alas acciones del usuario dinamicamente 

**Ejemplo**:

document.getElementById("miBoton").onclick = function() {
    alert("Haz hecho clic en el botón");
};

<button id="miBoton">Haz clic</button>

7. Describir al menos tres métodos para seleccionar elementos del DOM en JavaScript.

R//:
1. *getElementById*: // seleccionamos los elementos por id.

2. *getElementsByClassName*: // seleccionamos los elementos por clase.

3. *querySelector*:  // nos permite seleccionar elementos por id, class y tipo (etiqueta).


8. ¿Cómo se crea un nuevo elemento HTML y se agrega al DOM utilizando JavaScript?

R//:
De esta manera se crea
`document.createElement("h1")`// u otras etiquetas

`document.body`// se obtiene el body del documento

`cuerpoDelDocumento.appendChild(nuevoParrafo)`// se agrega el parrafo a el DOM con el metodo `.appendChild`


9. ¿Cuál es la importancia de la manipulación del DOM en la creación de aplicaciones web
dinámicas e interactivas?

R//:
igual a la respuesta de la pregunta **6**

10. Explicar brevemente los conceptos “event bubbling” y “event delegation” en el contexto 
de eventos del DOM.

R//:
por ejemplo si tienes un boton dentro de un div y haces click el evento no solo se queda en el boton sino que se propaga hasta el principio del div.

11. ¿Por qué son relevantes los conceptos “event bubbling” y “event delegation” en la 
gestión de eventos en páginas web con múltiples elementos interactivos?

R//:
Son relevantes por la eficiencia de codigo ,el manejo de elementos dinamicos , simplicidad y claridad etc.

