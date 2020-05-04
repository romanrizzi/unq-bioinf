
### TP 1 - Introducción a la bioinformática
Alumno: __Roman Rizzi__


##### RETO I: ¿Podrías buscar un ejemplo de macromoléculas que almacenen información sobre la ‘identidad’ de un organismo dado?

El ADN es una macromolécula compuesta de nucleótidos que se unen entre sí. Estas almacenan información genética de cada ser vivo.


##### RETO II: Propone una forma de expresar la información contenida en la estructura primaria de las proteínas usando tipos de datos de los lenguajes de programación que conocés.


La estructura primaria puede ser expresada usando un String o un Array de Strings ya que simplemente debemos listar en orden los aminoácidos que componen a la proteína.

##### RETO III: ¿ En qué tipo de datos podrías expresar la información de la estructura terciaria proteica?

La estructura terciaria podría representarse usando un grafo para indicar la forma en la que se va plegando la proteína.

##### RETO IV: Rosalind Franklin es una científica muy relevante, que tuvo menos reconocimiento del merecido. ¿Cuáles fueron sus contribuciones en este campo? ¿Qué nos cuenta su historia acerca del mundo de la ciencia?

Obtuvo imágenes de la estructura del ADN con una nitidez nunca antes vista mediante la técnica de difracción de rayos X. También realizó investigaciones sobre la utilización del carbón.

Su historia nos cuenta que el mundo de la ciencia era un ámbito machista donde no se les daba protagonismo a las mujeres y se las subestimaba. Lamentablemente, Rosalind Franklin no recibió crédito por sus descubrimientos sino que estos fueron compartidos sin su conocimiento.

##### RETO V: Propone en pseudocódigo un programa que prediga la estructura secundaria que adoptará cada residuo de la secuencia proteica dada, especificandola como H (si es una hélice), B (si es una hoja beta plegada) y L (si es un bucle o loop).

Asumiendo que la secuencia es un array de los aminoácidos y un hash donde las claves son los aminoácidos y los valores las preferencias, escribimos el siguiente pseudocódigo:

```ruby
  def estructura_secundaria(secuencia, preferencias)
    estructuras_posibles = { h: 0, b: 0, l: 0 }

    secuencia.each do |secuencia|
      preferencia = preferencias[secuencia]
      estructuras_posible[preferencia] += 1
    end

    estructuras_posibles.max_by { |k,v| v }
  end
```


##### RETO VI: ¿Qué hace distintos a dos individuos de una especie? Propone una forma de corroborar tu respuesta realizando un diagrama de un posible método computacional para dicho fin.

La diferencia está dada por pequeñas variaciones en la información genética de cada individuo. Una forma posible de corroborar esto es crear un programa que compare cadenas de ADN de distintos individuos formada por muchas combinaciones de cuatro nucleótidos A, C, G y T.

```ruby
def diferente_individuo?(cadena_a, cadena_b)
  cadena_a.each_with_index do |e_a, index|
    return true if e_a != cadena_b[index] 
  end

  false
end
```
