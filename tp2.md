### TP 2 - Introducción a la bioinformática
Alumno: __Roman Rizzi__
 
> ## La vida en tres dimensiones
 
#### ¿Por qué una célula querría destruir sus propias proteínas?
 
Una célula busca degradar sus propias proteínas para liberar los aminoácidos que la componen. Estos serán utilizados para formar otras proteínas o bien para generar energía.
 
#### ¿Qué información nos provee esta página?
 
Nos muestra información sobre la estructura tridimensional de una proteína y los resultados del estudio que se llevó a cabo para descubrir esta. Entre otras cosas, se incluye una visión 3D de la estructura, en que organismo está presente, su clasificación, autores, fecha de publicación del estudio, etc.
 
#### ¿Cómo se determinó la estructura de esta proteína?
 
La estructura fue determinada mediante el método de difracción de rayos X.
 
#### A la izquierda vemos una representación de la estructura de ubiquitina. ¿Qué significan las cintas, las flechas y las regiones angostas?
 
La imagen muestra la representación biología de la macromolécula. Esta puede provenir de las imágenes que se han tomado de esta o de la forma que se cree que tiene.
 
Las diferentes formas representan las cadenas, combinación, rotaciones y traducciones necesarias para formar la representación biológica completa de la macromolécula.
 
#### ¿Representa esa imagen a la realidad del sistema biológico?
 
No siempre, a veces puede ser aproximada por el autor o determinada mediante un programa.
 
#### La estructura 1UBQ fue “refinada a una resolución de 1.8 Angstroms”. Éste es el error asociado al experimento: mientras mayor es la resolución, menor es la certeza al determinar la posición de cada átomo. ¿Cuál es la utilidad y los condicionamientos de usar un modelo científico que sabemos inexacto?
 
> ## 3D View
 
#### En la pantalla principal vemos una representación de la estructura de ubiquitina. ¿Qué significan las cintas, las flechas y las regiones angostas?
 
Las diferentes formas representan las cadenas, combinación, rotaciones y traducciones necesarias para formar la representación biológica completa de la macromolécula.
 
 
#### ¿Qué diferencias y similitudes notamos respecto de la representación inicial?
bre cada átomo, incluyendo su nombre, carga, ocupacion, elemento, coordenadas en la representación, etc.
 
#### ¿Podríamos extraer de este archivo información sobre la estructura primaria de la proteína en cuestión? ¿Cómo se presenta dicha información y qué significa la representación? Desde el punto de vista computacional:¿de qué tipo de dato se trata esta información?
 
Si, los valores SEQRES listan los aminoácidos unidos de formar lineal. La información se presenta de la siguiente manera:
 
> SEQRES   1 A   76  MET GLN ILE PHE VAL LYS THR LEU THR GLY LYS THR ILE         
 
Siendo 1 el número de la cadena y A el identificador.
 
Desde el punto de vista computacional, esto se puede representar como un String o un Array.
 
 
#### ¿Considera que el formato PDB es útil para presentar los resultados del experimento?
Si bien inicialmente podemos ver la misma representacion biologica, esta vista nos permite rotar la macromolécula, ver distintas representaciones y los distintos aminoácidos que la componen.
 
#### En el menú de la izquierda hay opciones de distintos tipos de representación y formas de colorear la estructura tridimensional. ¿Para qué podría ser útil visualizar lo mismo de distintas maneras?
 
El coloreo es útil porque nos permite analizar la composición en base a distintos criterios, ya sea desde propiedades de los residuos, átomos, o cadenas hasta características como la simetría.
 
 
> ## PDB Format
 
#### ¿Qué información esperaría encontrar como resultado un experimento destinado a determinar la estructura terciaria de una molécula biológica?
 
Esperaría encontrar que átomos componen a la molécula y de qué forma están unidos entre si.
 
#### Podemos explorar el contenido del archivo que acabamos de descargar si lo observamos con un editor de texto. Haciendo clic con el botón derecho del mouse sobre el archivo descargado, usemos la opción ​Abrir con y seleccionemos el ​Bloc de Notas u otro editor de texto. ¿En qué consiste un archivo PDB?
 
El archivo PDB contiene la información necesaria para describir la estructura tridimensional de una molécula. En el archivo se incluye la descripción de la proteína y las estructuras de los ácidos nucleicos que incluyen las coordenadas atómicas, estructura secundaria y conectividad atómica.
 
#### Desplacémonos por el archivo hasta encontrar las líneas que comienzan con la palabra ATOM. ¿Qué tipo de información brinda esta sección?
 
Nos brinda información so
 
Es útil para almacenar y compartirlos rápidamente pero definitivamente no para presentarlo. Es muy difícil entender la información que muestra.
 
#### Observamos que la información respeta cierta estructura interna. ¿Cuáles son los beneficios y las limitaciones de imponer una estructura para comunicar los resultados de un experimento?
 
Las limitación principal es la falta de flexibilidad a la hora de agregar cosas que no estaban contempladas. Los beneficios de estandarizar la información de esta forma es la posibilidad de crear programas para utilizar este tipo de archivos y presentarlos de forma más amena para el lector.
 
#### Hemos visto que las proteínas tienen estructura tridimensional y hemos podido observar algunas características de las mismas. ¿Será igual con los ácidos nucléicos?
 
Si, también podemos visualizar ácidos nucleicos. Un ejemplo es el 2BG9.
 
 
#### Rosalind Franklin es una científica muy relevante, que tuvo menos reconocimiento del merecido. Contanos sobre los procedimientos que puso a punto Rosalind.
 
Rosalind Franklin puso a punto el método de difracción mediante rayos X, lo que permitió visualizar la estructura del ADN con una nitidez nunca antes vista.
 
 
