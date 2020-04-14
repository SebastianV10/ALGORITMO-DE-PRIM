# ALGORITMO DE PRIM

Utilizacion del algoritmo de Prim, con machine Learning.
    
### GRAFO

Un grafo G=(V,E) es un par de conjuntos donde los elementos de V se les
llama vertices, nodos, puntos y el conjunto E, es el conjunto de
aristas, este ultimo es un conjunto de pares de la forma (u,v) tal que
u,v pertenece a V. Por ejemplo:

La anterior imagen muestra un Grafo de los vertices V son
V=\{A,B,C,D,E\} y las aristas E=Xi tal que i=\{1,2,3,4,5\}, estos dos
grafos tienen la misma estructura pero sus formas son distintas, cumplen
con la teoria matematica del isomorfismo.\\\\

### ALGORITMO

Un algoritmo es una secuencia de instrucciones, al cual pueden llevarse
a cabo ciertos procesos y dar una respuesta a determinadas necesidades
y/o decisiones. Se trata de conjuntos ordenados y de finitos de pasos
que nos permiten resolver un problema o tomar una decisión. Por ejemplo.\\\\

### APRENDIZAJE SUPERVISADO

Es una de las 2 formas que las maquinas pueden entender un conjunto de
datos y se espera que aprendan algo util de ellos. Es la forma mas
comunmente utilizada a diferencia del aprendizaje NO supervisado,
incluye algoritmos como regresion lineal y logistica, maquinas de
soporte de vectores, entre otros.

Se llama asi por que el desarrollador actua como una guia para enseñar
al algoritmo las salidas a las que debe llegar. Es decir, la salida ya
es conocida. Es muy similar a la forma en la que un niño podria aprender
de un maestro. Requere que los posibles resultados del algoritmo ya sean
conocidos y que los datos utilizados para entrenar el algoritmo ya esten
etiquetados con las respuestas correctas. Por ejemplo: Una imagen
digital que muestra una serie de formas geometricas de colores
(Triangulos y cuadrados) que debemos unir en grupos de clasificacion y
color. Se le enseña a la computadora que las formas con 4 lados son
cuadrados y la forma con 3 lados son triangulos, tambien se le enseña
que luz emitida por un pixel se registra unos ciertos valores los cuales
identificaremos como rojo y otro valor como azul. con esto le habremos
enseñado a identificar triangulos y cuadrados de color azul y rojo.\\\\

### K-NN

Este algoritmo clasifica cada dato nuevo en el grupo que corresponda,
según tenga K vecinos más cerca de un grupo o de otro. Es decir, calcula
la distancia del elemento nuevo a cada uno de los existentes y ordena
dichas distancias de menor a mayor para ir escogiendo el grupo al que
pertenecer. Este grupo será el de mayor frecuencia con menores
distancias.

El K-NN es un algoritmo de aprendizaje supervisado que a partir de un
juego de datos inicial su objetivo será el de clasificar todas los
elementos nuevos. El juego de datos típico de este tipo de algoritmos
está formado por varios atributos descriptivos y un solo atributo
objetivo (también llamado clase). Por ejemplo: En la anterior imagen se
desea clasificar es el círculo verde. Para k = 3 este es clasificado con
la clase triángulo, ya que hay solo un cuadrado y 2 triángulos, dentro
del círculo que los contiene. Si k = 5 este es clasificado con la clase
cuadrado, ya que hay 2 triángulos y 3 cuadrados, dentro del círculo
externo.\\\\

### MATRIZ DE CONFUCION

es una herramienta fundamental a la hora de evaluar el desempeño de un
algoritmo de clasificación, ya que dará una mejor idea de cómo se está
clasificando dicho algoritmo, a partir de un conteo de los aciertos y
errores de cada una de las clases en la clasificaión. Así se puede
comprobar si el algoritmo está clasificando mal las clases y en qué
medida. Las matrices de confusión contienen información acerca de los
valores reales y las clasificaciones predichas hechas por cualquier
sistema de clasificación.\\\\

### CLASIFICADOR DE MACHINE LEARNING

Se trata una técnica muy utilizada en Machine Learning. para otorgar la
relevancia de una palabra en un documento de una colección a través de
una medida numérica. Esta medida numérica se utiliza para calificar la
relevancia de una palabra dentro de un documento a partir de la
frecuencia que aparece en el mismo. La idea en la que se basa esta
técnica es que si una palabra aparece frecuentemente en el documento,
debe ser importante y se le debe dar una puntuación alta. Sin embargo,
si una palabra aparece frecuentemente en otros documentos, probablemente
no sea un identificador único, y por tanto, se le debe asignar una
puntuación más baja.\\\\

### IMPLEMENTACION (KNN PARA CLASIFICACION, KNN PARA REGRECION)

El algoritmo k-nn se puede implementar en un sinfin de areas, redes de
cumputadores, matematicas,con muchos enfoques, para distintas mediciones
etc. Uno de los usos mas conocidos, es para clasificar las flores, segun
la medida de varias partes de la flor; al igual que este algoritmo en
esta ocacion lo usaremos para clasificar los datos, segmentarlos y
predecir el tamaño del error al evaluar los puntos cercanos.

Como primera medida vamos a usar las librerias scikit-learn de python,
que aunque el algoritmo en su instancia inicial sea aprendizaje
supervisado, estas librerias lo convierten en aprendizaje automatizado.
Consta inicialmente de escoger el porcentaje de datos los cuales van a
ser de test (20\%), y el resto de prueba (80\%), la libreria
scikit-learn convierte los datos seleccionados en el rango de -1,1 para
poder evaluarlos, y la libreria matplotlib la utilizamos para graficar.
Es importante destacar que aunque usemos la misma libreria para evaluar
datos, la clasificacion y la regrecion utilizadas aqui son procesos
separados, los cuales manejan los mismos datos pero procesos
independientes, confirmando la veracidad de los datos se imprime la
matriz de confucion.

Por ultimo, el grafo como enfoque inicial del problema lo generamos con
la libreria networkx la cual nos permite graficar tan solo con indicar
las aristas. Para este problema utilizamos un grafo completo, el cual la
libreria genera con tan solo indicar el numero de nodos.\\\\

### PROBLEMA

Tenemos la base de datos de cien (100) clientes de un almacen, buscamos
con esto clasificar los datos, y poder dar predicciones sobre los que
van a comprar; Al clasificar los datos, vamos a considerar que tenemos
identificacion, genero, edad, salario que devengan, y el valor verdadero
o falso que corresponde a si compro, o no lo hizo, como podemos apreciar
en la imagen de ejemplo de datos. Practicamente discriminaremos la
identificacion y el genero, realizando un analisis con las columnas de
edad, salario que devengas, y el valor que corresponde si com


 Los numeros posibles para ``numero de vecinos a tomar'' van desde 1 a 8;
sabiendo que si es mayor de 8 podemos tener Overflow. Por medio de las
graficas podra ver el error calculado al tomar diferente numero de
vecinos, con el fin de elegir el numero exacto con error minimo en el
rango.

    

> Este proyecto cuenta con licencia conforme a los terminos de la licencia MIT
