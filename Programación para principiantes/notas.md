# Notas Fundamentos de programación

> [!TIP]
> La programación es un arte y no solo de crear algortimos o aplicaciones, también es el arte de que otros programadores puedan leer tu código y sea legible, sin nececidad de escribir grandes comentarios o extensa documentación.

## Lenguaje de programación
### Bajo nivel
Es un lenguaje que se acerca más al binario, el cual es el lenguaje que entienden las computadoras (lenguaje máquina). Este tipo de lenguaje ofrece  como ventaja un mayor control sobre los recursos del hardware de los sistemas, pero presenta desventajas como una mayor complejidad en la programación y poca portabilidad entre diferentes sistemas. Ejemplos de estos lenguajes son el ensamblador y el lenguaje máquina.

### Alto nivel
Es un lenguaje más cercano al lenguaje que hablan los humanos. Abstrae mucho el manejo de recursos del hardware haciendo que se puedan concentrar más los programadores en la lógica de programación. Estos programas se traducen después al lenguaje máquina. Algunos ejemplos son Java, C++, python, Javascript, etc.

## Algoritmo
Es un proceso para resolver un problema, por lo general es ordenado y secuencial.
Siempre hay diferentes formas para resolver un mismo problema.
### Variable
Espacio en memoria para almacenar datos que necesitaremos usar para lograr hacer el algortimo
## IDE
Es un entorno de desarrollo integrado, es una aplicación de software que proporciona a los programadores todas las herramientas para la codificación, depuración y pruebas de software en un único entorno gráfico. 
Incluyen:
- Editor de texto
- Complilador y/o intérprete
- Depurador
- Gestor de proyectos
- Constructor de interfaz de usuario (UI Builder)
    - Como android Studio que puedes arrastrar las interfaces gráficas.
- Sistema de control de versiones

Ejemplos de estos son: Eclipse, Visual Studio, IntelliJ IDEA, PyCharm, etc.

## Editor de código
Son herramientas más ligeras. Te permiten escribir código y estos pueden tener extensiones que le dan más funcionalidades a tu experiencia de codificación. Tiene funcionalidades más reducidas a los IDE's. Ejemplo de estos son:
- Visual Studio Code
- Sublime Text
- Atom
- Nodepad++

## Dependencia
Una dependencia es un módulo, paquete, biblioteca o recurso externo que una aplicación o software necesita para funcionar correctamente. Estas son escensiales para proporcionar funcionalidades específicas dentro de una aplicación sin nececidad de reinventar la rueda, nos ayuda a no reescribir código desde cero. 
### Tipos de dependencias
1. Bibliotecas y Frameworks: Las aplicaciones suelen usar una biblioteca o frameworks externas que contienen código listo para usar y ayudar a crear cosas comunes como conexiones a bases de datos, manejo de sesiones de usuarios, creación de interfaces de usuarios, componentes, etc.
2. Módulos del Sistema: Servicios integrados como las librerías de Linux, las APIs de Windows o cualquier interfaz de programación de aplicaciones de los sistemas operativos.
3. Paquetes de Software: Software que necesita estar instalado en el sistema para que una aplicación funcione, como un servidor de bases de datos, un servidor web, intérprete de lenguaje de programación específico, etc.
4. Recursos Externos: Archivos de datos, imágenes, hojas de estilo CSS, scripts de JavaScript alojados en otros servidores, o APIs de terceros, como los servicios de Google Maps o API de Facebook.

### Dependencias de producción
Las que necesitamos para estar en producción
### devDependencies
Las que necesitamos solamente cuando estamos en desarrollo
