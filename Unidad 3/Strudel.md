const {visualid} = createParams('visualid')

setcps(119/60/4)

// ---- BATERÍA ----
const drums = stack(
  s("hh*2 hh*2 hh*2 hh*2")
    .visualid("drum_hh"),

  s("bd*2 ~ ~ ~")
    .visualid("drum_bd"),

  s("~ ~ sd ~")
    .visualid("drum_sd"),
)


// ---- PIANOS / ARMONÍA ----
const piano = stack(

  note("<[c3*4 c3*4]@2 [d3*4]>")
    .s("piano")
    .release(2)
    .visualid("piano_1"),

  note("<[c4*4 c4*4]@2 [d4*4]>")
    .s("piano")
    .release(2)
    .visualid("piano_2"),

  note("d#4, d#5")
    .s("piano")
    .release(2)
    .visualid("piano_3"),

  note("g#2, g#3")
    .s("piano")
    .release(2)
    .visualid("piano_4"),

  // ---- SECUENCIA PRINCIPAL ----
  note("<[c4, g4, c5, d#4]@1.5 [c4, g4, c5]@0.5 [d4, g4, a#3, a5]>")
    .s("piano")
    .clip(1)
    .release(0.05)
    .visualid("sec_1"),

  // ---- ACORDES DE APOYO ----
  note("<[g#2, g#3]@1.5 [[~] [a#2, a#3]]>")
    .s("piano")
    .release(2)
    .visualid("sec_1"),
)


// ---- MÚSICA COMPLETA ----
const Musica = stack(
  drums,
  piano
)


// ---- SALIDA PARA TOUCHDESIGNER ----
$: stack(
  Musica,
  Musica.osc()
)
