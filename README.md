- UTILIZAR STRING.XML SEGUN IDIOMAS


Le di click derecho a el string.xml pulse en Open Trasletions Edition ahi le di a Add Locale y añadi el idioma que queria, en mi caso aadi ingles y lo añadi


- CAMBIAR LAS IMAGENES DE DRAWABLE


En la carpeta drawable di clic derecho  , new, Vector Asset , en la pantalla que me aparecio le di a la opcion de Local file(SVG,PSD) en nombre puse el nombre del documento xml en el que queria cambiar la foto y en path seleccione la imagen nueva que queria.


- FUNCION DIFERENTE RANDOM


yo lo cambie asi:
 private fun rollDice() {
        val randomInt = listOf(1,2,3,4,5,6)
        val drawableResource = when (randomInt.random()) {
            1 -> R.drawable.dice_1
            2 -> R.drawable.dice_2
            3 -> R.drawable.dice_3
            4 -> R.drawable.dice_4
            5 -> R.drawable.dice_5
            else -> R.drawable.dice_6
        }

        diceImage.setImageResource(drawableResource)
    }
