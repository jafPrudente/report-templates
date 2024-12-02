# report-templates
En este repositorio se encuentran templates de LaTeX para reportes de laboratorio. Así mismo se encuentra un graficador en una notebook de python.

Para usar estos templates basta con clonar el repositorio y seleccionar la carpeta 'aps' o la 'std', dependiendo del resultado deseado. Dentro de las dos están los documentos y carpetas necesarias.

Se ha elegido separar cada sección en un documento separado que está en una carpeta correspondiente para que sea más fácil leer el código fuente y encontrar más rápido posibles errores. Estas secciones pueden ser fácilmente modificadas según las necesidades del usuario. 

En la carpeta 'Bibliography' está justamente la bibliografía en un archivo '.bib', para llenarlo se necesita usar el formato BibTeX, para ello basta con buscar la fuente en google scholar, dar click en 'Citar' y después en 'BibTeX'. Esto abrirá una página donde copiaremos el texto en ella y lo pegaremos en la sección correspondiente de este archivo '.bib'. Para hacer una referencia a esta nueva fuente basta escribir '\cite{nombreDeLaReferencia}', dicho nombre es el primer texto después del corcete de apertura.

Es importante señalar que todas las imágenes deben estar en la carpeta 'Images'. Así mismo es recomendable usar imágenes en formato '.pdf' puesto que no se pixelean al reescalarlas.

En ese sentido también se agrega una notebook en python para graficar. En este ejemplo se abre un archivo separado con tabuladores con cuatro columnas, las primeras dos tienen mediciones físicas, mientras que las últimas dos son las incertidumbres asociadas respectivamente. Se hace uso de la biblioteca 'pandas' para leer este archivo y de 'matplotlib' para graficarlo.

- Con 'plt.errorbar' se grafican puntos sueltos con barras de error asociadas. 
- Con 'plt.plot' se grafica una línea continua.
- El comando 'plt.xlabel' cambia la etiqueta del eje 'x', análogo con el eje 'y'.
- Con 'plt.legend' se posiciona el cuadro de las legends en cierta posición y además se cambia el tamaño de fuente.
- Con 'plt.tick_params' se cambia el tamaño de la fuente de los ejes.

En dado caso de necesitar hacer un ajuste con python mismo se puede revisar la documentación necesaria. Así mismo se puede modificar esta notebook para las necesidades de cada usuario y cada experimento.
