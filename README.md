# APUNTES M3 #

##### En estos apuntes explicaremos diferentes apartados, que son los siguientes: GITHUB, MARKDOWN, HTML, CSS y Diseño responsive #####

<hr>

## GITHUB ##

### *__Definición:__* ###
Git es un sistema de control de versiones, que nos ayuda a los usuarios a tener un historial completo de todas las modificaciones y avances que se han realizado. 
### *__Características:__* ###
 Este nos permite ir a versiones pasadas, ya que si esta mal lo hecho en el presente, volver a una versión reciente del pasado para no empezar de cero. Tambíen permite el trabajo por ramas, es decir, que si es un proyecto grupal, en este podemos trabjar cada uno diferentes ramas para después juntarlas. Hablando de esto, también hay una opción de clonar repositorios para asi trabajar de forma colaborativa y no molestar a tus compañeros. Por último, podemos trabajar de forma local, que esto evitará pérdidas en caso de que se pierda internet o algo así. Podremos trabajar en local con plataformas de desarollo colaborativas y asi alojar nuestro proyectos en la nube, con los repositorios remotos. 
### *__¿Como se utliza?__* ###
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
| git push origin main (“main” o el nombre de la rama a sincronizar)  - Se sincronizan los elementos incluidos en el anterior commit al repositorio remoto y rama indicadas en los puntos anteriores.. |
