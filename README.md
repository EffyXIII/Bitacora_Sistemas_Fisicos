# Bitacora_Sistemas_Fisicos

## Audio

Bueno, he tenido muchos problemas haciendo esto, sinceramente siento que carezco de algun tipo de conocimiento previo y que esto va rapidito pero x
aqui en la lucha. lo primero que intente fue realizar la cancion "Siento que merezco mas" de latin mafia. Imposible
de ahi empece a realizar una busqueda de distintas canciones que fuera mas posible para mi recrear (o al menos intentarlo)
finalmente llegue a MY EYES de travis scott
empece con el beat y tuve varias dificultades a la hora de separar los sonidos en el tiempo, luego de muchas pruebas logre medianamente arreglarlo haciendo distintas lineas para distintas parte
yo creo q quedo fino

ahora vamos con la melodia, espero no morir en el intento

la cosa no va mal, me esta gustando, pero tengo un gran problema, hacer las siguientes secuencias de acordes, y no tenog mucho tiempo
### el codigo va asi:

setcps(119/60/4)

$: stack(
  s("hh*2 hh*2 hh*2 hh*2"),
  s("bd*2 ~ ~ ~"),
  s("~ ~ sd ~")
)

$: stack(
  note("d2*2 d2*2").s("piano").release(2),
  note("a2*2 a2*2").s("piano").release(2),

  note("c4").s("piano").release(2),
  note("g4").s("piano").release(2),
  note ("c5").s("piano").release(2),
  note ("d#4").s("piano").release(2)
 
 // note("f#3*2 f#3*2").s("piano").release(2)
)
