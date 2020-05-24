### TP 4 - Introducción a la bioinformática
Alumno: __Roman Rizzi__
 
 
#### Trabajaremos con las secuencias del citocromo c de nueve organismos, listados en la tabla de abajo. Además de su denominación taxonómica, deberíamos conocer su nombre común: intentemos completar la tabla.
 
| Secuencia  | Nombre taxonómico   |  Nombre común |
|:--------:| :------: | :-------: |
| NP_061820.1 | Homo sapiens |  Humano |
| NP_001072946.1 | Gallus gallus |  Gallo |
| NP_001065289.1 | Pan troglodytes | Chimpancé común  |
| NP_001157486.1 | Equus caballus |  Caballos |
| NP_001183974.1 | Canis lupus familiaris |  Perro |
| AEP27192.1 | Gorilla gorilla | Gorila occidental |
| XP_024245566.1 | Oncorhynchus tshawytscha |  Salmón real, |
| NP_001086101.1 | Xenopus laevis |  Rana de uñas africana |
| NP_477164.1 | Drosophila melanogaster |  Moscas de la fruta |
 
 
#### ¿Cuán sencillo será alinear dos o más secuencias a mano? ¿Cuánto influirán el número de secuencias a alinear, su longitud, y la similitud entre ellas?
 
La dificultad se incrementa a medida que la cantidad de secuencias y la longitud de estas aumenta. No es una tarea sencilla ya que todavía no contamos con alguna forma mecánica de hacerlo y debemos ir probando a ojo.
 
#### ¿Son parecidos los citocromos c de humano y gallo?
 
La suma de residuos idénticos en posiciones equivalentes al alinear las dos secuencias nos hace pensar que son parecidos. Comparten 92 elementos en las mismas posiciones y solo difieren en 13.
 
#### ¿Qué teorías subyacen a este análisis?
 
> Por lo que el término homología se usa solo cuando el antepasado común es lo suficientemente reciente como para que la información de la secuencia haya retenido suficiente similitud como para hacer inferencias evolutivas (Park et al. 1998)
 
> Suele ser mejor para evaluar relaciones evolutivas lejanas la comparación a nivel de secuencias de proteínas, mientras que para relaciones más cercanas suelen utilizarse las secuencias de ácidos nucleicos que codifican para las mismas, ya que estas suelen ser menos informativas que las secuencias proteicas (Pearson, 1996).
 
#### ¿Cómo nos ayuda la evolución a explicar sus similitudes y diferencias?
 
La evolución explica que las poblaciones van diferenciándose debido a las variaciones al azar y el ambiente que determinan el grado significativo en el que los organismos se reproducen y sobreviven, y dado suficiente tiempo, esto lleva a una acumulacion de cambios.
 
### Clustal
 
#### Podemos elegir verlo en colores (​Show Color)​ . ¿Qué indican los colores?
 
Los residuos de las secuencias que son idénticos o similares reciben un color. Este es seleccionado según las propiedades químicas del residuo.
 
#### ¿Qué indican el guión (-), los dos puntos (:) y el asterisco (*)?
 
Los guiones representan introducen huecos en el alineamiento, representando adiciones y deleciones.
 
Los dos puntos indican que el residuo para esa posición se repite en la mayoría de las cadenas comparadas.
 
El asterisco indica que el residuo en esa posición es el mismo para todas las cadenas comparadas.
 
#### A simple vista, ¿se conserva la secuencia del citocromo c en los organismos?
 
Si, si nos guiamos por lo mencionado en la pregunta anterior, hay una gran cantidad de asteriscos, lo que indica que hay gran conservación.
 
#### ¿Creeríamos que todos los organismos se asemejan por igual al resto, o se pueden identificar grupos de mayor similitud? Si es así, ¿tienen sentido?
 
No, no todos los organismos se asemejan por igual al resto. Esto tiene sentido ya que a medida que los organismos van evolucionando, estos van acumulando cambios que los hacen diferentes del resto.
 
#### ¿Qué evidencias nos aportaría este análisis, a la luz de la evolución?
 
Nos muestra que muchos organismos comparten ancestros comunes, que estos fueron divergiendo para adaptarse y la acumulacion de cambios los ha hecho diferentes entre sí.
 
#### A juzgar por los organismos participantes, ¿cuáles creería que deberían estar más agrupados en el árbol filogenético?
 
Deberían estar agrupados por especies y descendencia:
 
- Humano, Gorila occidental, chimpancé común
- Gallo
- Salmón, Rana
- Caballo
- Perro
- Moscas
 
#### Observemos el árbol filogenético. ¿Concuerda con lo esperado? ¿De qué organismos son los citocromos c más parecidos? ¿Cómo se explica?
 
Los citocromos c más parecidos son del Salmón y la Rana, y del Humano y el Chimpancé. Concuerda con los esperado y también agrega información sobre ancestros comunes.
