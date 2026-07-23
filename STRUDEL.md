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
