***MÓDULO SOBRE HTML, CSS Y RESPONSIVE DESIGN***

1. ¿Qué significa HTML y cuál es su función en el desarrollo web?

R//:
significa:  "Hypertext Markup Language" (Lenguaje de Marcado de Hipertexto, en español)
la funcion es crear una estructura ordena del contenido.

2. ¿Cuál es la estructura básica de un documento HTML? Describir las etiquetas 
esenciales.

R//:
<!DOCTYPE html> //Esta es la que nos define que es una estructura web
<html lang="en">// dentro de estas va toda la estructura del proyecto
<head>// La informacion que va en esta etiqueta no la ve el usuario lo que hace es contener el titulo para la web, hojas de estilos. 
    <meta charset="UTF-8">// Que tipo de caracteres son "arabe", "chino"etc.
    <meta name="viewport" content="width=device-width, initial-scale=1.0">//En este va la descripcion de la pagina.
    <title>Document</title>//Titulo de la pagina web.
</head>
<body>// El cuerpo de la pagina web
    
</body>
</html>

3. ¿Qué es CSS y cuál es su propósito en el desarrollo web?

R//:
Es un lenguaje de estilos para describir la presentacion visiual de una pagina, el proposito es que las hojas de estilos sean aparte de los archivos html y tener medidas, colores y tamaños.

4. ¿Qué son selectores CSS, cuáles son los principales tipos de selectores y porqué es 
importante entender la especificidad en el contexto de las hojas de estilo en cascada 
(CSS)? Describir al menos tres tipos de selectores CSS y cómo la especificidad afecta 
a la aplicación de estilos en un proyecto de desarrollo web Frontend. Proporcionar 
ejemplos de situaciones en las que se utiliza la especificidad de selectores para resolver 
conflictos de estilos.

R//:
Los selectores en css son patrones que se utilizan para aplicar estilos a la estructura html  

*selector de tipo*
    selecciona todos los elemento de tipo especifico por ejemplo si es una p cogeria todos lo p.
*Selector de Clase:*
    selecciona todos los elementos que tengan el atributo class ejemplo .mi__clase todos los que tengan esa class.
*Selector de ID:*
    selecciona un unico elemento con el atributo id ejemplo #mi__id.

5. Explicar las diferencias entre los estilos en línea (inline), estilos internos (embedded) y 
estilos externos (external) en CSS. Indicar cuál de los tres estilos es el recomendado 
usar y por qué

R//:
**Estilos en linea**
Los estilos en linea se aplican directamente a el html con el atributo style  por ejemplo: <p style="color: blue;">Texto en azul.</p> 

**Estilos internos**
Los internos se definen dentro de la etiqueta por ejemplo: 
<head>
    <style>
        p {
            color: red;
        }
    </style>
</head>

**Estilos externos**
Los estilos externos se almacenan en un archivo separado con extension .css y se  enlaza con el html ejemplo:
<head>
    <link rel="stylesheet" type="text/css" href="estilos.css">
</head>    es mas recomendado usar estilos externos para que estilos solo se encargue de presentacion.

6. ¿Qué es flexbox y cómo se utiliza para el diseño de páginas web?

R//:
Flexbox, también conocido como Flexible Box Layout  es un diseño en css que permite crear diseños mas eficientes y flexibles (responsive)

*ejemplo*

.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

7. Explicar cómo se emplean las propiedades flexbox y explicar la función de las 
principales propiedades en la creación de diseños flexibles.

R//:
a el conteedor principal es a el que si le asigna lo flexible para poder trabajar con los elemento internos mas facilmente.

*ejemplos*:
//Hace que un elemento se haga a el lado del otro//

.contenedor {
    display: flex;
}

//Hace que los elementos se filen horizontalmente//

.contenedor {
    flex-direction: row;
}

//Hace que haya un espacio entre cada elemento dependiendo el tamaño del contenedor//

.contenedor {
    justify-content: space-between;
}

8. ¿Qué es CSS Grid Layout y en qué se diferencia de flexbox?

R//:
 Es otro modelo de diseño en CSS que permite la creación de diseños bidimensionales tanto en filas como en columnas estructuras de cuadrícula más complejas la diferencia es que Flexbox está diseñado para trabajar en una dimensión (fila o columna) de manera eficiente

9. Proporcionar un ejemplo de cómo crear una cuadrícula sencilla con CSS Grid.

R//:
    .grid-container {
        display: grid;
        grid-template-columns: repeat(3, 100px); 
        grid-template-rows: repeat(3, 100px);    
        gap: 10px;
        }

    .grid-item {
        background-color: #3498db;
        color: #ffffff; 
        padding: 20px; 
        text-align: center;
        }


10. ¿Qué significa el diseño responsivo en el contexto del desarrollo web?

R//:
significa que puede tener la capacidad de adaptarse a el tamaño de diferentes dispositivos

11. Enumerar al menos tres técnicas o estrategias utilizadas para lograr el diseño 
responsivo en una página web.

1. *Media Queries*//@media only screen and (max-width: 600px)
2. *Imágenes Flexibles*//max-width: 100%;
3. *Unidades Relativas*//font-size: 2rem; , font-size: 1.2em;

