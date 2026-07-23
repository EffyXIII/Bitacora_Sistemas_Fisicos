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


va mejorando el asunto y la optimizacion del codigo, ahora el problema es que los acordes no suenan en los tiempos que deseo y no encuentro como arreglarlo



LOGRE LO QUE QUERIA. AQUI EL CODIGO



He estado progresando mucho en lo que busco y siento que cada vez se hacerca mas, lastimosamente dude que de el tiempo para poder avanzarlo y mejorarlo mucho mas. lo di todo
al final el codigo se queda asi

setcps(119/60/4)

$: stack(
  s("hh*2 hh*2 hh*2 hh*2"),
  s("bd*2 ~ ~ ~"),
  s("~ ~ sd ~")
)

$: stack(
  note("<[c3*3 c3*3]@1.5 [[c3*2][d3*2]]>").s("piano").release(2),
  note("<[c4*3 c4*3]@1.5 [[c4*2][d4*2]]>").s("piano").release(2),

  note("d#4, d#5").s("piano").release(2),
  note("g#2, g#3").s("piano").release(2),


//secuencia principal
  note("<[c4, g4, c5, d#4]@1.5 [[c4, g4, c5] [d4, g4, a#3, a5]]>").s("piano").clip(1).release(0.05),

//Acordes de apoyo 
  note("<[g#2, g#3]@1.5 [[~] [A#2, a#3]]>").s("piano").release(2), // Volumen más suave para que quede de fondo



  
// INTENTO BUENO. PORFIN, pero vamos a probar algo mas
  //note("<[c4, g4, c5, d#4] [[c4, g4, c5] [d4, g4, a#3, a5, a#5]]>").s("piano").release(2),
  
  
  //intento 3
  //note("<[[[c4, g4, c5, d#4]]] [[c4, g4, c5] [d4, g4, a#3, a5]]>").s("piano").release(2),
  
  //intento 2
  //note("[c4, g4, c5, d#4] [c4, g4, c5] [d4, g4, a#3, a5]").s("piano").release(2),

  //intento 1 de acordes
  //note("c4").s("piano").release(2),
  //note("g4").s("piano").release(2),
  //note ("c5").s("piano").release(2),
  //note ("d#4").s("piano").release(2)
 
 // note("f#3*2 f#3*2").s("piano").release(2)
)



casi me voy sin pushear esto y voy a llegar tarde por hacerlo. pero me di cuento que me estaba pegando un tiro en el pie con los corchetes 

setcps(119/60/4)

$: stack(
  s("hh*2 hh*2 hh*2 hh*2"),
  s("bd*2 ~ ~ ~"),
  s("~ ~ sd ~")
)

$: stack(
  note("<[c3*4 c3*4]@2 [d3*4]>").s("piano").release(2),
  note("<[c4*4 c4*4]@2 [d4*4]>").s("piano").release(2),

  note("d#4, d#5").s("piano").release(2),
  note("g#2, g#3").s("piano").release(2),


//secuencia principal
  note("<[c4, g4, c5, d#4]@1.5 [c4, g4, c5]@0.5 [d4, g4, a#3, a5]>").s("piano").clip(1).release(0.05),

//Acordes de apoyo 
  note("<[g#2, g#3]@2 [A#2, a#3]>").s("piano").release(2), // Volumen más suave para que quede de fondo



  
// INTENTO BUENO. PORFIN, pero vamos a probar algo mas
  //note("<[c4, g4, c5, d#4] [[c4, g4, c5] [d4, g4, a#3, a5, a#5]]>").s("piano").release(2),
  
  
  //intento 3
  //note("<[[[c4, g4, c5, d#4]]] [[c4, g4, c5] [d4, g4, a#3, a5]]>").s("piano").release(2),
  
  //intento 2
  //note("[c4, g4, c5, d#4] [c4, g4, c5] [d4, g4, a#3, a5]").s("piano").release(2),

  //intento 1 de acordes
  //note("c4").s("piano").release(2),
  //note("g4").s("piano").release(2),
  //note ("c5").s("piano").release(2),
  //note ("d#4").s("piano").release(2)
 
 // note("f#3*2 f#3*2").s("piano").release(2)
)
