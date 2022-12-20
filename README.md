# APUNTES M3 #

##### En estos apuntes explicaremos diferentes apartados, que son los siguientes: GITHUB, MARKDOWN, HTML, CSS y Diseño responsive #####

<hr>

## GITHUB ##

### *__Definición:__* ###
Git es un sistema de control de versiones, que nos ayuda a los usuarios a tener un historial completo de todas las modificaciones y avances que se han realizado. 

### *__Características:__* ###
 Este nos permite ir a versiones pasadas, ya que si esta mal lo hecho en el presente, volver a una versión reciente del pasado para no empezar de cero. Tambíen permite el trabajo por ramas, es decir, que si es un proyecto grupal, en este podemos trabjar cada uno diferentes ramas para después juntarlas. Hablando de esto, también hay una opción de clonar repositorios para asi trabajar de forma colaborativa y no molestar a tus compañeros. Por último, podemos trabajar de forma local, que esto evitará pérdidas en caso de que se pierda internet o algo así. Podremos trabajar en local con plataformas de desarollo colaborativas y asi alojar nuestro proyectos en la nube, con los repositorios remotos. 
 
### *__¿Como se utiliza?__* ###
1. Tenemos que crear un repositorio nuevo: <img width="948" alt="image" src="https://user-images.githubusercontent.com/113420749/195032040-7805ae32-8613-401a-806a-386f39355278.png">
Cuando pongas la opción de nuevo repositorio deberás poner el nombre que quieras al repositorio. La opción de ser público o privado es dependiendo lo que quieras. La mejor opción es un repositorio público, ya que este lo podemos publicar en GitHub Pages. También podemos poner la opción de *README*, que es ideal si queremos un repositorio que se crea automáticamente y que también se inicializa. Si no queremos eso, no tenemos que marcar esa opción, se usará para crear un repositorio nuevo desde cero en local. A contiuación hay una tabla donde se explica los diferentes casos de si no ponemos el archivo *README*:

| Ponemos README |
| -------------- | 
| Para crear un repositorio local nuevo y sincronizarlo con un repositorio de GitHub no inicializado (vacío). Hacerlo desde la carpeta “raiz” del repositorio local, no desde fuera.
| git init - Inicializamos el repositorio GIT en la carpeta donde estamos situados.|
| git add "archivo” o  git add . - Elementos que van a incluirse en la nueva versión  Si se incluye el wildcard “.” se incluirán todos los archivos del repositorio.
| git commit -m "añadir título"  - Descripción de la versión o fecha, o cualquier indicador que defina qué cambios se han hecho en la versión
| git push origin main (“main” o el nombre de la rama a sincronizar)  - Se sincronizan los elementos incluidos en el anterior commit al repositorio remoto y rama indicadas en los puntos anteriores.. |


| Repositorio local nuevo desde línea de comandos |
| ----------------------------------------------- | 
| Para clonar en el disco duro local un repositorio ya creado e inicializado de GitHub y poder trabajar en local, tendremos que tener instalado GIT en el disco duro.
| echo "# BORRAR" >> README.md - Creamos el archivo readme.md con el contenido que queramos.|
| git init - Inicializamos el repositorio GIT local vacío en la carpeta donde estamos situados.
| git add README.md  - Añadimos el archivo readme al repositorio local
| git commit -m "first commit" - Commit es un conjunto de cambios que se realizan en los archivos del repositorio (modificar, añadir, eliminar, mover, renombrar, etc). Creamos el paquete de archivos a sincronizar con el repositorio remoto (se incluirán los archivos que hayamos hecho “add” anteriormente y le ponemos nombre identificativo a la nueva versión con el parámetro -m.. |
| git branch -M main  - Asociamos la versión a la rama de desarrollo que queramos. La rama por defecto es “main”. |
| git remote add origin -  https://github.com/Alfie/BORRAR.git  asociamos un repositorio remoto indicando un identificador (origin) y su URL
| git push -u origin main - Subimos los cambios al repositorio remoto y rama indicadas en los puntos anteriores.|


| Sincronizar un repositorio local local ya existente desde línea de comandos: |
| -------------- | 
| Navegamos en local hasta la carpeta raíz del repositorio local a vincular con el repositorio vacío recién creado en GitHub.
| git init - Inicializamos el repositorio dentro de la carpeta raiz del mismo|
| git remote add origin - https://github.com/AlbertoDeSantos/BORRAR.git. Una vez situados en la carpeta, añadimos como origen de ese repositorio al repositorio vacío de GitHub.
| git add . Añadimos todos los archivos al repositorio local
| git commit -m "first commit" - Commit es un conjunto de cambios que se realizan en los archivos del repositorio (modificar, añadir, eliminar, mover, renombrar, etc). Creamos el paquete de archivos a sincronizar con el repositorio remoto (se incluirán los archivos que hayamos hecho “add” anteriormente (en esta primera ocasión TODOS) y le ponemos nombre identificativo a la nueva versión con el parámetro -m.|
| git branch -M main - Asociamos la versión a la rama de desarrollo que queramos. La rama por defecto es “main”.
| git push -u origin main - Subimos los cambios al repositorio remoto y rama indicadas en los puntos anteriores.|


Para importar un repositorio que ya tenemos, debemos ir a ese repositorio y a CODE. Ahí copiamos el link y lo guardamos. Más tarde vamos a crear un nuevo repositorio y le damos a la opcón de importar uno nuevo.

### *__¿Que es GitHub Pages?__* ###
GitHub Pages sirve para publicar repositorios. Para subir uno, debemos hacer los siguientes pasos:
1. Ir a _AJUSTES_
2. Ir a pages abajo a la izquierda y escogemos a qué rama asociar “pages” (por defecto “main”) y a qué carpeta (por defecto “root”) y aplicamos configuración con “Save”: 


![image](https://user-images.githubusercontent.com/113420749/195041244-9e6c8c2e-abbc-4841-ab5d-fdb85f012ef2.png)

Con todo esto, ya tenemos nuestro link para publicar nuestro repositorio.

<hr>

## MARKDOWN ##

### *__Definición:__* ###
Es un lenguaje de marcas llamdo "Markdown" que es usado por GitHub.

### *__Etiquetas básicas:__* ###
Primero de todo tenemos los encabezados, donde podemos elegir el tamaño según los # que pongamos delante de la palabra.

# Encabezado 1 (H1)
## Encabezado 2 (H2)
### Encabezado 3 (H3)
###### Encabezado 4 (H4)

También podemos utilizar diferentes estilos de letras. 
- Itálica o cursiva: *texto* o _texto_ (utilizamos una barra baja al inicio y final de palabra o frase)
- Negrita: **texto** o __texto__ (utilizamos dos barra bajas al inicio y final de palabra o frase)

Aparte de estos dos estilos de letras, podemos hacer listas, tanto ordenadas como desordenadas.
- Para hacer lista __ORDENADA__:
1. Poner el uno, punto y después un espacio
2. Das a enter y sigue haciendo
3. Hasta el número que quieras
4. Únicamente dando al enter
5. Para parar de hacer la lista debemos dar doble enter y ya

- Para hacer una lista __DESORDENADA__: 
+ Utilizar giones (signos de resta, suma) y también el asterisco de multiplicación.

Este lenguaje nos permite hacer muchas cosas, como poner enlaces hacia otras páginas.
Para hacer esto tenemos que poner el título que queramos entre "[]" y seguido el link que queremos enlazar entre parentesis. "()"
[Gotham Knights](https://www.gothamknightsgame.com/es-es)

También nos permite poner imágenes:

![image](https://user-images.githubusercontent.com/113420749/196377503-95a4c030-0728-4d0b-ba6c-1a95cbb6093a.png) Y pie de foto también

__¿QUE TENEMOS QUE HACER PARA PEGAR UNA IMAGEN?__
1. Escoger imagen
2. Descargarla
3. Copiarla
4. Pegarla en el git

Este sistema también nos permite hacer tablas, para ordenar diferentes factores:

![image](https://user-images.githubusercontent.com/113420749/196378388-98ccd5ca-074e-48b2-b04d-b46706280030.png)

- Los dos puntos se usan para alinear las columnas (izquierda, centrado, derecha).
- No es necesario que estén alineadas verticalmente. Solo a nivel visual para claridad del código.
- Se han de poner al menos tres guiones para separar cada encabezado

| Primero | Segundo | Tercero |
| :------:| :------:| :------:|
| Messi | Cristiano | Neymar |
| Jordan | Kobe Bryant | Lebron James |

Por último podemos hacer unas listas de verificación:

![image](https://user-images.githubusercontent.com/113420749/196380034-9b9c0016-629f-44d4-8481-a883da0f7d21.png)

- [ ] A
- [x] B
- [ ] C

<hr>

## ````HTML```` ##

````  ¿QUE ES HTML?  ````

HTML són les sigles de Hyper Text Markup Language. És un llenguatge de marques per descriure documents web (pàgines web) més usat actualment en el món web.

```` ESTRUCTURA: ````

- html: Elemento raíz del documento.
- head: Espacio destinado a contener información del documento. 
- title: Título descriptivo de la pàgina web. Normalmente aparece en la barra del navegador, también és el texto que se guarda en los marcadores del navegador (lista de direcciones de interès). 
- meta: Metainformación de la página. Podemos poner diversas marcas <meta>, que dan información no visible del documento. 
- body: Cos o contingut del document. 


EJEMPLO DE HEAD

```` 
<head>
   <meta charset="utf-8"/>
   <title> Mipaginaweb  </title>
</head>
````

EJEMPLO DE BODY
Lo que se ve en medio del body es un coementario, que no aparecería en la página web

````
 <body> 
<!-- Contenido de la web --> 
</body> 
````
EXEMPLE HTML FINAL:

````
<!DOCTYPE html >
<html>
   <head>
<meta charset="utf-8"/>
  	<title>Mipaginaweb </title>
   </head>
   <body>
<!-- Contenido de la web -->
   </body>
</html>
````

````Etiquetas````

Las etiquetas básicas de HTML son casi lo mismo que en GitHub, los encabezados por ejemplo, la linea separatoria y para hacer un salto de linea. Ahora pondré las que son diferentes:

- Las listas desordenadas son aquellas en las que el orden de los ítems no es relevante, como en una lista de compras. Estas son encerradas en un elemento <ul> (unordered list).
- Las listas ordenadas son aquellas en las que el orden sí es relevante, como en una receta. Estas son encerradas en un elemento <ol> (ordered list).

-  Párrafos (<p>). Se utilizan para encerrar párrafos de texto, entendiendo como párrafo un conjunto de frases relacionadas entre sí. Son elementos de bloque.

- Enlaces (<a>). Para convertir algún texto dentro de un párrafo en un vínculo, sigue estos pasos:


¿Que es el Fontawesome?

Esto son iconos que puedes implementar en la ventana de tú página web. Un ejemplo de esto puede ser esto:

![image](https://user-images.githubusercontent.com/113420749/197497276-35314abc-23cb-4ffd-a8eb-c378a52cb643.png)
La imagen del gato de GitHub es lo que puede modificar el Fontawesome.

COMO SE UTILIZA:

````<script src="https://kit.fontawesome.com/09f87768b9.js" crossorigin="anonymous"></script>````

Copia tu “kit's code” dentro de la sección <head> de cada página en tu proyecto donde quieras usar fontawrsome mediante ese kit. La parte subrayada dependerá del ID de tu kit’s code.

Código de ejemplo:
````
     <!doctype html>
      <html>
        <head>
          <!-- Poner el código de tu kit aqui directamente tal y como lo propone Fotawesome -->
          <script src="https://kit.fontawesome.com/09f87768b9.js" crossorigin="anonymous"></script>
        </head>

        <body>
          <i class="fa-solid fa-thumbs-up fa-5x"></i> <!-- El código lo da la plataforma en el propio icono -->
        </body>
      </html>
````

<hr>


## CSS ##

### *__Definición:__* ###
CSS en español «Hojas de estilo en cascada», es un lenguaje de diseño gráfico para definir y crear la presentación de un documento estructurado escrito en un lenguaje de marcado.

### *__Características:__* ###

*FUNCIÓN:*

Para evitar que HTML fuese el responsable de la parte estética y visual de la web se idearon las hojas de estilo y el lenguaje CSS (Cascading Style Sheets).
Mientras que HTML estructura del documento e indica a los navegadores la función de un elemento en concreto (un vínculo, un título,....), el CSS da instrucciones al navegador sobre como ha de mostrar un elemento concreto: estilo, espaciado, posición..
Aunque (X)HTML tiene marca relacionadas con la visualización y presentación en la web, es mejor no usarlas dado que estas etiquetas mezclan estructura y presentación del documento. CSS no es un lenguaje de programación como JavaScript ni un lenguaje de etiquetas como HTML.

*VENTAJAS:*

- Posibilidad de mantener el código
- A nivel de diseño, CSS es más potente que las etiquetas de diseño de (X)HTML.
- CSS es un lenguaje sencillo.

También se pueden definir diferentes hojas de estilo para un solo documento (X)HTML, por ejemplo, un estilo para la página web cuando se visita desde un ordenador y otra para cuando queramos imprimirla. Además, se pueden reutilizar desde diferentes documentos (X)HTML.

*DESVENTAJAS:*

El gran inconveniente es que no todos los navegadores se comportan de la misma forma ante una hoja de estilo dado que algunos no cumplen con los estándares establecidos. Así, obligan al programador a crear diferentes hojas de estilo. 

 *ESTRUCTURA:*
 
Una estructura es como vamos a poner la sintaxis CSS para que funcione. Esta estructura contiene selectores que un selector nos sirve para definir a qué elemento o elementos queremos aplicar las declaraciones de la regla. Las declaraciones son las diversas características que han de cumplir los elementos que concuerdan con el selector. A cada propiedad de cada declaración le ponemos el valor que sea necesario.
 
*TIPOS DE SELECTORES*
 
 - Selector de elementos:  Corresponde con todos los elementos de este nombre en la página. El siguiente ejemplo afectaría a TODOS los elementos <a> del documento HTML:
 ````
 /* All <a> elements. (Nota) */
a {
   color: red;
} 
````

- 
