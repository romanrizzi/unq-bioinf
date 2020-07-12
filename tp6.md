### TP 6 - Introducción a la bioinformática
Alumno: __Roman Rizzi__

#### RETO I: Detalla las tácticas y/o metodologías que deberían utilizarse para darles una respuesta a los padres del niño.

#### a) Dadas las secuencias de Mosca, humano y Moscahumano ¿Qué criterios se les ocurren para comparar las secuencias? ¿Qué resultados obtienen del análisis anterior?

Viendo los alineamientos de los 3 en Clustal, podemos observar que los tres comparten la mayoría de los elementos y esto es todavía mayor si comparamos solamente al humano y a bart mosca. Podríamos decir que bartmosca conserva mas del humano que de la mosca.

#### b) ¿Qué resultado esperaría obtener si utilizara el resto de las secuencias en el análisis? ¿Por qué?

Utilizando la misma táctica que en el punto anterior, podemos ver como las similitudes son mucho menores ya que las muestras han acumulado suficientes mutaciones como para no parecerse entre si.

#### RETO II: Mediante el uso del servidor de ​IQtree ​(Trifinopoulos et al. 2016)​, confecciona los árboles filogenéticos para los alineamientos obtenidos en el punto II.

#### a) Como vemos, el servidor nos permite elegir el modelo de sustitución ¿A qué se refiere?

Nos permite elegir la forma en la que se producen las sustituciones entre las determinadas secuencias a fin de "corregir" la distancia entre secuencias y estimar el numero de sustituciones que han ocurrido. Elegir un modelo lo mas cercano al verdadero comportamiento de la evolución de las secuencias es clave para construir un buen árbol filogenético.


##### b) ¿Qué es el Bootstrap? ¿De qué manera nos habla de la calidad de nuestro árbol? ¿Cómo influye el número de Bootstraps en el resultado?

Bootstrap es un método para inferir que tan fiable es nuestro árbol. El bootstrap value nos indica que tantas veces pudimos observar la misma rama del arbol al realizar la reconstrucción filogenética.

##### c) Interpreten los resultados obtenidos, mediante la visualización de los árboles con la herramienta ​FigTree​. ¿Es necesario realizar algún paso extra, previo a la interpretación del árbol? ¿Por qué?

Es necesario alinear las secuencias antes de generar el árbol filogenético para poder reconstruirlo correctamente.

Según los resultados, `NP_061820.1_cytochrome_c_[Homo_sapiens]` es el ancestro mas cercano a `bartmosca` ya que están en el mismo nivel en el árbol.