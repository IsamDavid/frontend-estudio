# Notas de HTML y CSS
## ¿Qué es HTML y CSS?
### HyperText Markup Language (HTML)
El lenguaje de etiquetas de hipertexto es el código con el que se estructura una página web. (el esqueleto)
### Cascading style sheets
Las hojas de estilo en cascada es el lenguaje que le da colores, forma, tamaño, formato a los elementos de nuestro esqueleto (el código html). 
### Motores de renderizado
Cada navegador tiene su propio motor de renderizado para poder "traducir" nuestros archivos de código html y css a algo que puede entender el navegador y lo transforma en pixels (algo visual) para que nosotros lo podamos visualizar. 
| Navegador | Motor |
| --- | --- |
| Chrome | Blink |
| Edge | Edge html |
| Safari | Webkit |
| Firefox | Gecko
#### Pasos de los motores de los navegadores para tranformar el código
1. Pasar los archivos a objetos (DOM)
    El Document Object Model (DOM) es la representación de nuestro código HTML en una estructura de árbol. El motor de 
    ![Ejemplo de código en la estructura de árbol - DOM](imagenes-de-apoyo/ejemploDom.png)

    Y el equivalente de este árbol en código lo puedes ver [aquí](DOM-ejemplo.html)
    
    ***El DOM representa la relación entre las etiquetas de los archivos HTML.***
    El CSSDOM (Cascade Style Sheet Object Model) es lo mismo que el DOM pero con los archivos CSS.
2. **Calcula el estilo** correspondiente a cada nodo del DOM
    Toma cada uno de los estilos css que tenga cada uno de los nodos del árbol y los añade.
3. **Cálcula las dimensiones** de cada nodo y dónde va en la pantalla. 
4. Pinta o renderiza los diferentes elementos como **cajas o contenedores** (las etiquetas que se muestran en el ejemplo)
5. Agrupa todas las cajas en diferentes capas para **convertirlas en una imagen que se renderiza en pantalla**
## Anatomía de un documento HTML y sus elementos
Cada elemento del código HTML se conforma del siguiente contenido:

- Etiquetas
    - Este es la representación de un elemento html. Tiene una etiqueta de apertura y una de cierre.
    - Ejemplo:
        ```html
        <h1></h1>
        ```
- Contenido
    -   Es el texto o elemento que se encierra entre la etiqueta. Puede que tenga texto o no (Depende de la etiqueta)
    - Ejemplo
        ```
        <h1>Este es el contenido</h1>
        ```
- Atributos
    - Estos manejan el comprtamiento de un elemento, se escriben dentro de la etiqueta de inicio.
- Elementos vacios
    - Hay etiquetas que no tienen contenido y etiqueta de apertura, por lo general se les agrega atributos y este determina el comportamiento de dicha etiqueta
    - Ejemplo
        ````
        <img src="ejemplo.jpg" alt="ejemplo">
        ```
- Anidamiento
    Estas son etiquetas dentro de otras etiquetas, esto es regular en HTML. Esto dependera de la estructura que necesitemos.
    - Ejemplo
        ```
            <section>
                <h1>Hola Mundo</h1>
            </section>
            <!-- Una lista no organizada -->
            <ul>
                <!-- Elementos de la lista no ordenada -->
                <li>Increíble</li>
                <li>Maravilloso</li>
                <li>Genial</li>
        ```
## Elementos de la estructura principal
Para  ver la estrucutra de un archivo html da click [aquí](/estructura.html)
### Etiqueta Doctype
Esta etiqueta especifica que el archivo se va a manejar con la versión 5 de HTML.
### Etiqueta html
Esta etiqueta define el elemento raíz de un archivo HTML. Es la etiqueta madre y todos los demás elementos deben de estar dentro de esta etiqueta. Aquí se especifica el lenguaje de la página web con la propiedad **lang**
### Etiqueta head
Esta etiqueta define la **metainformación**, lo que quiere decir que estará toda la información que no es contenido de una página web. Aquí van los archivos CSS, JavaScript, el título y la imagen (favicoon) que aparece en la pestaña de navegación. Aquí también va más información que es importante para los ***motores de busqueda*** como Google.
## HTML SEMÁNTICO
En html tenemos la etiqueta ```<div>```, esta etiqueta nos sirve como contenedor pero carece de valor semántico lo que significa que no significan nada para los motores de busqueda como google.
### Etiquetas Semánticas
En el siguiente [archivo](/EtiquetasSemanticas.html) tenemos un ejemplo de etiquetas.
Aquí tenemos el ejemplo con una imagen de cómo estas etiquetas podrían estar estructuradas en nuestra página web ![imagen de semántica html](imagenes-de-apoyo/ejemploSemántica.png)
***Es importante aclarar que todo esto podemos hacerlo con div pero no tendríamos las ventajas que se mencionan a continuación***
### Ventajas de utilizar HTML semántico
- Ayuda a tu sitio a ser accesible, esto es porque el sitio va a leer la etiqueta que es y ayuda con los programas de accesibilidad.
- Mejora tu posicionamiento (SEO)
- Código más claro, legible y mantenible, haras que otros desarrolladores o tu yo del futuro pueda entender a qué se refiere esa parte del contenido, ya que no tendrás puras etiquetas ```<div></div>``` anidadas.
- Ayuda a buscadores (como Google a encontrar tu página)
