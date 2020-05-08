### TP 3 - Introducción a la bioinformática
Alumno: __Roman Rizzi__


#### RETO I: Enumerá las diferencias que existen entre una célula procariota y eucariota.


 - Las células procariotas no tienen un núcleo definido y su material genético se encuentra disperso en el citoplasma. En cambio, las eucariotas tienen un núcleo definido por una membrana que contiene el material genético.

 - Las procariotas son más pequeñas y su tamaño va entre 1 y 10 micrones mientras que las eucariotas entre 10 y 100.

 - La división celular procariota es directa, principalmente mediante fisión binaria mientras que en las eucariotas sucede por mitosis y meiosis.



#### RETO II: Crea un programa sencillo en algún lenguaje de programación que conozcas que imprima una cadena de ARN codificante para el siguiente péptido (cadena corta de aminoácidos).

```ruby
def imprimir_arn(peptido, tabla)
  valores_validos = 'UCAG'

  cadena = []
  elemento = []
  peptido.each do |p|
    elemento << p if valores_validos.includes? p
    
    if elemento.size == 3
      cadena << tabla[elemento]
      elemento = []
    end
  end

  cadena
end
```

#### RETO III: Crea un programa sencillo en algún lenguaje de programación que conozcas que permita identificar las regiones promotoras de un gen, en una secuencia dada de ADN, considerando que tal región comienza y termina en con la caja TATA.

```ruby
def imprimir_indices(peptido)
  caja_valida = 'TATA'

  regiones = []
  indices_region = []
  caja = ''
  peptido.each_with_index do |p, idx|
    caja << p
    
    if caja.size == 4 && caja == caja_valida
      if indices_region.size.zero?
        indices_region << idx +1
      else
        indices_region << idx - 3
        regiones << indices_region
        indices_region = []
      end

      caja = ''
    end
  end

  indices_region
end
```

#### Diseñá un juego de mesa o un videojuego (hecho con la herramienta que más te guste) temático sobre expresión génica, con sus reglas y resúmen. Tené en cuenta que lo vas a tener que compartir con la clase.

El juego trata de una célula que acaba de expulsar cadenas de ARN, el jugador debe clickear el botón para hacer aparecer a los ribosomas y así crear proteínas. Si el jugador no llega a hacer aparecer los 3 ribosomas a tiempo, pierde el juego.