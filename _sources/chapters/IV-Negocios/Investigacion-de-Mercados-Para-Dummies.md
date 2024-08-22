# Cómo hacer Investigación de mercados con inteligencia artificial 

Todos los negocios necesitan hacer investigación de mercado.

Imagínate que te subes a un avión y el piloto te dice que los monitores de vuelo están descompuestos. No hay comunicación con las torres de control, no hay forma de saber cómo será el clima en el trayecto y no hay forma de saber si vas en la ruta correcta y llegarás al aeropuerto correcto (o a algún aeropuerto siquiera). ¿Te subes?

¡Por supuesto que no!

La investigación de mercado es la forma en la que un negocio obtiene información sobre su entorno. Puede ser de manera formal (con encuestas, entrevistas, focus group y observación de las métricas) o informal (la observación simple). Todas las empresas la tienen, porque todas reciben información de su entorno.

Son nuestros monitores de vuelo.

## Cuando una marca de pasteles instantáneos decidió quitarle ingredientes a su producto y ¡vendieron más que nunca!

> *A veces no hacer nada es hacerlo todo
-* Teniente Harina
> 

En los años 50s toda la economía en Estados Unidos estaba creciendo.

Cuando la economía está creciendo, tener un producto medianamente innovador era garantía de que te harías millonario. A pesar de eso, General Mills no lograba levantar las ventas de su mezcla para hacer pastel en casa. Era sin duda un producto innovador

Lo que hicieron a continuación, convirtió a las mezclas en un éxito y revolucionó el mercado para siempre.

La necesidad era real: las amas de casa estaban hambrientas de soluciones que les ahorren tiempo de las tareas del hogar. Así que los ejecutivos decidieron contratar a Ernest Dichter para hacer una investigación de mercado. Dichter fue el pionero de los **grupos de enfoque**, que juntan en un sólo cuarto a un grupo de amas de casa para encontrar las verdaderas causas del problema.

Tras entrevistar a más de cien amas de casa, Dichter encontró que la razón por la que no compraban era **culpa**. ¡Ellas querían participar en la elaboración del pastel! Un producto “demasiado fácil” de preparar las hacía ver cómo flojas y no cómo amas de casa de verdad (recuerda que eran los años 50).

La solución: quitar ingredientes a la mezcla y dejar que las amas de casa aporten más al proceso.

Ahora las amas de casa debían incluir huevo y leche a la mezcla para que quedara completa. Para la empresa esto significaba menos costos, pero más importante es que las ventas por fin crecieron. La mezcla era ahora más valiosa, porque permitía hacer un pastel, ser parte del proceso y terminarlo con facilidad.

Así de importante es tener un buen conocimiento del mercado.

[]

## Pero ¿Un estudio de mercado es sólo hacer preguntas?

Si, pero no es fácil hacer las preguntas correctas.

Para hacer las preguntas correctas necesitas entender el problema que estás solucionando, al cliente para quien estás haciendo tu solución y cómo estás contribuyendo a la solución. El problema y tu solución son importantes porque ayudan a identificar lo que debes cambiar para hacer tu oferta más valiosa, pero esas son cosas que están bajo tu control. Lo que no está control es tu cliente y sus decisiones.

Hay cosas de tu cliente que puedes aprender observando, pero otras se las vas a tener que preguntar directamente.

- ¿Por qué te eligió en lugar de la competencia?
- ¿Cómo usa tu producto / servicio?
- ¿Percibe algún riesgo de que tu producto no cumpla su promesa?

En realidad el cielo es el límite. 

Puedes preguntarle lo que se te ocurra a tus clientes. El problema es que la mayoría de nosotros no sabemos diseñar las preguntas correctas y los clientes no tienen ningún incentivo para decirnos la verdad. Hace un par de años, si no tenías el don de diseñar encuestas o no tenías a tu disposición a un buen sociólogo, mala suerte.

Pero hoy podemos apoyarnos de la IA para crear una encuesta increíble.

## Usemos a chatGPT para diseñar una encuesta en el estilo del Mom Test

En 2013, Rob Fitzpatrick publicó “The Mom Test”.

En este libro, explicaba cómo cuando diseñamos una pregunta para una investigación de mercado, solemos mezclar objetivos y acabamos queriendo publicitar nuestro producto o servicio. El resultado es que hacemos las preguntas “amañadas” para que nos den una respuesta positiva. Pero eso no es útil para nosotros: queremos que si alguien odia nuestro producto, nos lo diga con todo lujo de detalle.

En otras palabras, quieres que incluso tu mamá te diga si hay algo en tu producto que necesitas cambiar.

El libro está lleno de ejemplos, geniales. Si los estudias, puedes transformar las preguntas en tu estudio de mercado para que cumplan con el objetivo y mejores la calidad de tus respuestas.

O puedes decirle a chatGPT que haga esa modificación por ti.

Estos son mis pasos:

- Define lo que quieres conocer de tus clientes.
- Redacta o elige las preguntas que quieres hacerles.
- Transformalas al estilo del mom test.

Hagamos un ejemplo.

### Define lo que quieres conocer de tus clientes

Digamos que tienes una e-commerce de ropa y quieres identificar puntos de fricción en el proceso de compra. En este caso hay miles de elementos que puedes probar por tu cuenta haciendo pruebas A/B. Pero también hay aspectos que no puedes observar y que tienes que únicamente puedes saber si se los preguntas directamente al cliente.

Tres ejemplos de esto serían:

- **La calidad percibida del producto.** ¿Por qué no la puedes medir con los datos de interacción? Como es una tienda en línea, hay detalles que las fotos no pueden mostrar. Algunos clientes lo podrían poner en las reseñas, pero muchos probablemente sólo dejen de comprar. Adios cliente y adiós datos.
- **Experiencia de soporte al cliente.** Esto incluye aspectos como la facilidad del menú, la rapidez y utilidad de las respuestas y la satisfacción general.
- **La experiencia del checkout.** Hay aspectos como qué tan fácil o difícil fue usar el carrito de compra, si les gustaría incluir opciones de pago o la claridad en costos de envío.

Puse ejemplos de cosas que no podrías medir usando pruebas A/B, pero tal vez también desees investigar aspectos que se pueden medir en pruebas A/B usando una encuesta.

La razón principal de esto es que el tiempo es limitado y sólo puedes hacer pruebas limitadas a la vez. Muchos expertos recomiendan sólo usar una prueba a la vez, pero los modelos de panel y de diferencias en diferencias en este libro te pueden ayudar a hacer más. Aún con esto, tal vez no quieras usar tu tiempo y recursos de las pruebas A/B en hacer estudios triviales.

### Redacta o elige las preguntas que quieres hacer

Comencemos definiendo lo que queremos conocer.

Usa el siguiente prompt en chatGPT o el mejor modelo de inteligencia artificial al que tengas acceso.

```
Ayúdame a hacer las preguntas para un estudio de mercado.

Giro: e-commerce de ropa.
Mercado meta: Gen-Z de Mexico y latinoamerica.
Propuesta unica de valor: Te damos puntos por tu ropa vieja que te dan descuentos en la nueva. Estamos luchando para combatir el fast fashion.

Te daré información sobre lo que quiero conocer de ellos y me darás 15 opciones de preguntas.

- **La calidad percibida del producto.**
- **Experiencia de soporte al cliente.** Incluye aspectos como la facilidad del menú, la rapidez y utilidad de las respuestas y la satisfacción general.
- **La experiencia del checkout.** Hay aspectos como qué tan fácil o difícil fue usar el carrito de compra, si les gustaría incluir opciones de pago o la claridad en costos de envío.
```

Normalmente deseamos que la extensión de nuestro estudio sea suficientemente larga para que nos de información valiosa, pero no tan larga para que la contesten hasta acabarla (con sinceridad). Por eso le pedimos 15 preguntas, pero seleccionamos sólo las mejores.

Modifica el prompt anterior con los datos de tu negocio o emprendimiento y sigamos.

### El mom test, explicado

Te voy a ahorrar leer un libro entero en este texto de 3 minutos.

El mom test es una técnica donde las preguntas se diseñan para que no te contesten lo que piensan que quieres oír. Digamos que queremos preguntar cómo califican la calidad de la ropa en nuestra e-commerce. Hay muchas razones por las que alguien que conteste el cuestionario no quiere contestarte con la verdad.

- Tal vez sienten que decir algo negativo sería muy confrontativo.
- Tal vez realmente quieren agradarte.
- O simplemente les estás haciendo una pregunta en la que tienen que pensar demasiado su respuesta y te acaban contestando lo que sea.

En todos estos casos, el culpable no es el que responde, eres tú.

Para entender mejor el mom test, observa estas preguntas. Son ejemplos de lo que no se debe hacer. ¿Puedes identificar por qué son malas preguntas?

- ¿Crees que {X} es buena idea de negocio?
- ¿Comprarías {X}?
- ¿A qué precio te parece justo comprar {X}?

Estás preguntas están mal planteadas porque alguien que no estaría dispuesto a comprar tu producto te puede fácilmente decir que si, es buena idea. Tu te vas feliz con la impresión de que tienes la idea más genial de negocio y al final creas algo que a nadie le interesa. *Sad to be you*.

En lugar de eso, puedes preguntar

- ¿Cuales son los mayores problemas que enfrentas cuando haces {actividad relacionada con X}?
- Cuéntame sobre la última vez que necesitaste algo similar a {X}. ¿Que solución utilizaste?
- ¿Que has pagado anteriormente por productos o servicios similares a {X}? ¿Cómo decidiste que valía la pena ese precio.

La razón por la que estas preguntas son mejores es que están diseñadas para sacarle la verdad al encuestado.

Las preguntas del *mom test* se enfocan en experiencias pasadas y decisiones reales. Hacer esto refleja mejor cómo se comportaría el usuario en una situación específica. Además, son preguntas que ayudan a entender el contexto y las motivaciones del usuario.

Ahora transformemos nuestras preguntas.

## Transformando nuestro estudio al estilo del mom test

Para mi, el mom test es una metodología fácil de aprender, pero difícil de implementar.

Me toma mucho tiempo y trabajo hacer esas modificaciones. Afortunadamente los modelos de lenguaje grandes tienen ya cargada en su entrenamiento la información relacionada al mom test, porque hay miles de posts de blogs sobre el tema (y probablemente el libro mismo ahí venga cargado. Lo que antes nos tomaba horas, lo podemos hacer en minutos.

Puedes hacerle un prompt sencillo:

```
redacta las preguntas en el estilo del mom test
```

Listo.

Tu encuesta ahora genera información más valiosa.

## Referencias

Fitzpatrick, R. (2013). *The Mom Test: How to talk to customers & learn if your business is a good idea when everyone is lying to you*. CreateSpace Independent Publishing Platform.

General Mills. (1950s). *Marketing research on cake mix*. 

Dichter, E. (1950s). *Focus group studies on cake mix for General Mills*.

Harina. (2022, March 10). *A veces no hacer nada es hacerlo todo*. En *Harina* (temporada 1, episodio 5). Amazon Prime Video.


<div style="height: 100vh"><script src="https://cdn.jsdelivr.net/ghost/signup-form@~0.1/umd/signup-form.min.js" data-label-1="inferenciacausal.com" data-background-color="#ffffff" data-text-color="#000000" data-button-color="#154957" data-button-text-color="#FFFFFF" data-title="Escribe tu primer paper de Economía" data-description="Todos los meses recibe un tutorial de econometría, un análisis de un artículo y una guía" data-icon="https://marionomics.com/content/images/size/w192h192/size/w256h256/2024/08/2.svg" data-site="https://marionomics.com/" data-locale="es" async></script></div>

_Elaborado en el ejercicio de año sabático UJED_
