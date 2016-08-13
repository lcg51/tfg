# README #

Esta es una plantilla para LaTeX que puede ser utilizada para escribir los TFG del grado de Ingeniería Multimedia de la Universidad de Alicante.

Para descargarla, ve a https://bitbucket.org/ppernias/tfg_im/downloads. Una vez descargado y descomprimido el fichero correspondiente se habrá creado un directorio nuevo con varios ficheros y subdirectorios en él. Cámbiale el nombre al directorio principal por el que quieres utilizar. 

La plantilla está en revisión, por lo que se recomienda utilizar siempre la última versión de la misma.

## Descripción ##
La plantilla incluye, a modo de capítulo de introducción y otro con el nombre de "marco teórico" ejemplos de escritura de diversas estructuras en LaTeX, como son:
 
* Títulos para Capítulos y Secciones
* Listas numeradas y no numeradas
* Tablas
* Cómo insertar código fuente para su visualización en LaTeX
* Cómo insertar citas bibliográficas.
* Cómo insertar imágenes/ figuras y sus referencias

La plantilla genera automáticamente:

* la portada a color (con los elementos identificativos del grado de Ingeniería Multimedia de la UA. Si se va a imprimir esta portada aparte, eliminar la referencia correspondiente de la plantilla)
* Una segunda portada en blanco y negro con los datos de autor, y tutor(es)
* Índice general
* Índice de figuras, tablas y listados de código
* Estructura genérica para un TFG siguiendo las normas de la EPS de la UA.
* Bibliografía en formato APA
* Anexos

La plantilla está pensada para una impresión final del TFG a doble cara, con márgenes diferentes para páginas pares e impares.

Además, genera líneas de cabecera para aquellas páginas que deben tenerla, así como paginación en números romanos o arábigos allí donde corresponde hacerlo de cada manera.

La plantilla posee muchas otras características que pueden ser modificadas revisando el código LaTeX correspondiente.

## NOTAS importantes: ##

Hay dos portadas:

* Primera portada a color con los elementos identificativos del grado de Ingeniería Multimedia de la Escuela Politécnica de la UA. En realidad, esta portada es un PDF que se incrusta en la primera pagina del TFG sobre un fondo a color. Este PDF ha sido generado aparte, poniendo en él los elementos necesarios para una adecuada presentación. Se adjunta en este repositorio el fichero de esa portada en formato PSD para su edición con el software Photoshop o similar y posterior generación del PDF personalizado.

* Segunda portada en b/n. Esta portada recoge la información suministrada en el fichero principal de la plantilla ("tfg_im.tex") en la sección "Información sobre el TFG". Allí se puede indicar el autor del TFG, el título y subtítulo del TFG y el nombre y departamento del/los tutor/es. Comentar o borrar aquello que no se precise.

## Gestión de la bIbliografía ##

Se ha añadido un subdirectorio ("bibliografia") con un fichero de tipo **BIBTEX** con algunos ejemplos de entradas bibliográficas. Este fichero está enlazado con la plantilla para su compilación conjunta. Se debe utilizar este fichero para la recopilación de la bibliografía por parte del alumno y su gestión con el software que el alumno elija para ello. En el texto hay ejemplos de cómo se debe citar una fuente que exista en ese fichero.

## Software para la escritura del TFG en LaTeX ##

Existe mucho software para escribir el LaTeX dependiendo del S.O. que se esté utiiizando. Una búsqueda por Internet permitirá encontrar el más adecuado a los gustos del autor. En http://tex.stackexchange.com/questions/339/latex-editors-ides hay una buena lista de editores LatTeX. Un ejemplo podría ser:

**Para Windows**

  * TexWorks que se encuentra en http://www.tug.org/texworks/

**Para OSX**

  * La suite TexShop / Bibtex que puede ser descargada en http://pages.uoregon.edu/koch/texshop/
  * TexWorks: http://www.tug.org/texworks/

**Para Linux**

  * TexStudio http://texstudio.sourceforge.net/ (Recomendado por el prof. Juan Ramón Rico)
  * TexMaker: http://alternativeto.net/software/texmaker/

Los editores LaTeX suelen venir acompañados de un software para la gestión de la bibliografía. Este software permite ir registrando las fuentes bibliográficas en el formato de fichero BIBTEX (usar el mencionado anteriormente) y generar las referencias necesarias que hay que poner en LaTeX para que aparezcan correctamente en el texto y al final en el capítulo de "Bibliografía" y que lo hagan en el formato correcto.

## AVISO ##
Esta plantilla no es perfecta. Puede ser mejorada con las aportaciones de muchos. Por favor, si puedes mejorarla, hazlo y comenta en los foros de este repositorio lo que has hecho. El resto de nosotros te estaremos muy agradecidos.

## Fuentes ##
La plantilla está basada en otras similares y en aportaciones de profesores de la UA:

* Plantilla para TFG de la U. de Granada: http://grados.ugr.es/informatica/pages/infoacademica/tfg/plantillas/plantilla_tfg_latex
* Aportaciones de Rafael Carrasco (DLSI Univ. de Alicante)

*
**Pedro Pernías Peco. Coordinador Académico del grado de Ingeniería Multimedia. Alicante, diciembre de 2014** 
*

--
**Ampliación**

Pedro Pastor (DSLSI) propone:

"... utilizar la clase {scrbook} en lugar de la clásica {book} puede traer algunas complicaciones si no se domina el lenguaje. {scrbook} es más moderna (e incluye bastantes paquetes que en {book} hay que incluir aparte, pero si se quiere "customizar" algo hay que saber cómo, y no se hace igual que en {book} ( que es la que explican la mayoría de los manuales). Es decir, habría que estudiarse el manual de KOMA-Script.
Por ejemplo, se que incluye algunos paquetes AMS para escribir matemáticas, pero no se si falta alguno"

Por ahora, creo que es mejor dejar {scrbook} ya que cambiarlo por {book} genera una serie de errores en la compilación LaTeX que obligarían a cambiar muchas otras cosas y hasta que no las estudie, no se el efecto que tendría. 

Además, ha sugerido sustituir el paquete "color" por "xcolor" y reubicar la llamada al paquete "hyperref". Estas modificaciones se han incorporado  a la versión actual de la plantilla.