#  Proyecto end to end para e-commerce

El objetivo de este proyecto es realizar un proyecto end to end para poner en práctica varios conocimientos.
Dentro de este proyecto tenemos dos carpetas principales una que son src en donde subiremos todos los scripts que usaremos durante el código.
Y la otra carpeta que tendríamos serían los notebooks en el que desarrollaremos y comentaremos cada uno de los rotados obtenidos por los diferentes análisis que vayamos haciendo

1. Dentro de la carpeta src tenemos cuatro archivos el orden es el siguiente.
   * Data loader funciona para descargar nuestros datos del origen correspondiente
   * Data cleaner funciona para la limpieza de los datos así como la validación de los mismos es el intermedio entre la capa bronze y silver del esquema medalion
   * Data save solamente es una función que nos servirá para guardar los datos y cargarlos cuando sea necesario.
   * Finalmente stars squema builder nos permite transformar nuestros datos de una manera que sea fácil de consultar para el usuario final es el puente entre la capa silver y la capa gold del esquema medalion.

2. Dentro de la carpeta notebooks encontraremos cuatro archivos principales describimos el funcionamiento y el propósito de cada uno en el escrito correspondiente sin embargo daremos un resumen rápido de qué trata cada uno.
   * 01 carga de datos este notebook se encarga de procesar los datos en cada una de las capas correspondientes para su limpieza y para la entrega final a la persona que se encargará de hacer los análisis
   * 02 de análisis de datos tiene el objetivo más exploratorio su objetivo es describir a grandes rasgos qué información tenemos y qué podemos describir con ella sin entrar tanto en temas estadísticos
   * 03 análisis estadístico esta parte se encarga del análisis más riguroso haciendo pruebas de hipótesis análisis de correlación y respondiendo preguntas desde un punto de vista más teórico.
   * 04 transfer learning el objetivo de notebook es entrenar un modelo para poder realizar análisis de sentimiento de acuerdo a la review que den de un producto de esta forma podemos comprender cuál es el sentimiento a la hora de escribir una review.

De forma independiente cada uno de los notebooks tienen la descripción más detallada sobre lo que se esté realizando cómo se está realizando y para qué se está realizando, espero este proyecto pueda servir de ayuda  -> :) 
