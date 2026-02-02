# Experimentos y Pruebas A/B

> *Outsized returns often come from betting against conventional wisdom, and you can't know whether you're right until you try. Big winners pay for so many experiments.*
> - Jeff Bezos

> *If your experiment needs statistics, you ought to have done a better experiment.*
> - Ernest Rutherford

En mayo de 2024 mi esposa abrió un negocio de extensiones de pestañas en Mazatlán. Como cualquier negocio nuevo, necesitaba clientes. Y como cualquier negocio nuevo en 2024, la forma más rápida de conseguirlos era con publicidad en Instagram.

Pero había un problema: no sabíamos qué tipo de anuncio funcionaría mejor. ¿Debería el anuncio mostrar una foto de antes y después? ¿O una foto del resultado final? ¿Debería incluir el precio o no? ¿Debería mencionar una promoción de apertura o no?

En lugar de debatir, decidimos hacer un experimento. Creamos $2^3 = 8$ variantes de anuncios combinando tres variables: tipo de foto (antes/después vs. resultado final), si se incluía el precio o no, y si se mencionaba la promoción de apertura o no. Cada variante se publicó como un anuncio independiente en Instagram con el mismo presupuesto.

```{figure} ../../figures/anuncios.png
---
width: 100%
name: fig-anuncios
---
Las 8 variantes de anuncios de Instagram que probamos para el negocio de pestañas. Cada anuncio combinaba tres variables binarias: tipo de foto, precio visible y mención de promoción.
```

Los resultados fueron sorprendentes. El mejor anuncio costaba alrededor de 40 pesos mexicanos por cada cliente potencial (lead), mientras que el peor costaba más de 200 pesos por lead. Es decir, el peor anuncio era **cinco veces más caro** que el mejor. Sin el experimento, habríamos elegido un anuncio al azar --y probablemente no habría sido el mejor.

Este es el poder de los experimentos: en lugar de adivinar, **medimos**.

## Los experimentos son el *gold standard* de la ciencia

Si has usado las plataformas de publicidad de Meta, Google o TikTok, ya has hecho pruebas A/B aunque no lo sepas. Estas plataformas están diseñadas para experimentar. Pero los experimentos no se limitan a la publicidad. Empresas como Stripe, Netflix, Amazon y Booking.com corren miles de experimentos al año para optimizar desde el color de un botón hasta la estructura de precios de sus productos.

La idea es simple: si quieres saber si un cambio tiene un efecto, divide a tu audiencia en dos grupos al azar. A un grupo le muestras la versión A (el control) y al otro la versión B (el tratamiento). Después comparas los resultados. Si la diferencia es lo suficientemente grande, puedes concluir que el cambio tuvo un efecto causal.

La barrera más grande para experimentar no es técnica, sino de **tiempo**. Diseñar un buen experimento, esperar a que se recolecten suficientes datos y analizar los resultados toma tiempo. Y en un entorno de negocios donde todo es urgente, el tiempo es el recurso más escaso.

Además, no todo se puede probar con un experimento. No puedes asignar aleatoriamente a las personas a ser fumadoras o no fumadoras para estudiar el efecto del tabaco en la salud. No puedes asignar aleatoriamente a los países a tener democracia o dictadura para estudiar el efecto del sistema político en el crecimiento económico. Hay preguntas donde los experimentos simplemente no son éticos o factibles.

Pero cuando sí puedes experimentar, **deberías hacerlo**. Los experimentos son la herramienta más poderosa que tenemos para establecer causalidad.

## ¿Por qué se usan experimentos para hacer inferencia causal en los negocios?

Imagina esta escena: estás en una junta con tu equipo de marketing. Llevan 45 minutos debatiendo si el título de la página de inicio debería decir "La mejor solución para tu negocio" o "Haz crecer tu negocio hoy". El director de marketing cree que la primera opción es mejor porque suena más profesional. El diseñador prefiere la segunda porque es más directa. El CEO quiere una tercera opción que nadie más apoya.

¿La solución? Dejen de debatir y hagan un experimento. Muestren la versión A a la mitad de los visitantes y la versión B a la otra mitad. Después de una semana, vean cuál genera más conversiones. Listo.

Los experimentos se usan en los negocios por al menos cuatro razones:

1. **Eliminan la duda sobre la causalidad.** Si asignaste aleatoriamente a los usuarios a ver una versión u otra, cualquier diferencia en los resultados se debe al cambio que hiciste, no a otros factores. No hay variables confusoras de las cuales preocuparse.

2. **La matemática es simple.** Para analizar un experimento bien diseñado, en muchos casos solo necesitas comparar promedios. ¿El grupo B compró más que el grupo A? Si la diferencia es estadísticamente significativa, tienes tu respuesta. No necesitas modelos complicados ni supuestos heroicos.

3. **Los resultados son más interpretables.** Cuando le dices a un directivo "el nuevo diseño aumentó las ventas un 12%", esa persona entiende exactamente lo que significa. Compara eso con explicarle los coeficientes de una regresión con variables instrumentales.

4. **Pueden ser más baratos que las juntas interminables.** El costo de un experimento en una plataforma de publicidad digital es relativamente bajo. El costo de oportunidad de que cinco personas pasen una hora debatiendo sin datos es mucho mayor.

## ¿Qué pasa cuando no se puede hacer un experimento?

Siempre es útil empezar pensando en el **experimento ideal**, incluso cuando sabemos que no lo podemos ejecutar. Joshua Angrist y Jörn-Steffen Pischke, dos de los econometristas más influyentes de nuestra era, sugieren en su libro *Mostly Harmless Econometrics* (2009) que siempre comiences cualquier estudio preguntándote: "¿Cuál sería el experimento ideal para responder esta pregunta?"

La razón es que al pensar en el experimento ideal, identificas con claridad cuáles son los supuestos necesarios para que tu análisis sea válido. Si no puedes hacer el experimento, al menos sabes qué estás asumiendo cuando usas métodos observacionales.

Es como tener un mapa del tesoro. Tal vez no puedas tomar el camino directo porque hay un río de por medio, pero al menos sabes dónde está el tesoro y puedes buscar rutas alternativas. Sin el mapa, estás caminando a ciegas.

En el resto de este libro veremos varias de esas "rutas alternativas": diferencias en diferencias, variables instrumentales, regresión discontinua y matching. Cada una de estas técnicas intenta imitar lo que haría un experimento aleatorio, pero usando datos observacionales. Y cada una tiene sus propios supuestos y limitaciones.

## Aunque no lo creas, hay preguntas que no se pueden resolver ni aún con un experimento

Hay preguntas que parecen simples pero que son imposibles de responder con un experimento, no por razones éticas o prácticas, sino por razones lógicas.

Considera esta pregunta: ¿cuál es la mejor edad para emprender?

Pierre Azoulay y sus coautores publicaron en 2020 un estudio fascinante que encontró que la edad promedio de los fundadores de startups exitosas en Estados Unidos es de 42 años. Pero, ¿significa esto que ser mayor te hace mejor emprendedor?

No necesariamente. El problema es que la edad viene acompañada de muchas otras cosas: experiencia laboral, red de contactos, capital acumulado, conocimiento del mercado, madurez emocional. No puedes asignar aleatoriamente la edad a las personas. Y aunque pudieras, no podrías separar la edad de todas las variables que vienen con ella.

Esto es lo que los estadísticos llaman un problema de **identificación**. La edad no es una variable que puedas manipular independientemente de todo lo demás. Es inseparable de la experiencia, el capital y muchas otras cosas.

Reconocer los límites de lo que podemos saber es tan importante como saber responder preguntas. Un buen analista no solo encuentra respuestas; también sabe cuándo una pregunta no tiene respuesta con los datos disponibles.

## Ejemplo: El efecto de las búsquedas pagadas en las ventas

Uno de los modelos de negocio más exitosos de la historia es el de Google. La empresa gana la mayor parte de sus ingresos subastando espacios publicitarios en sus resultados de búsqueda. Cuando buscas "zapatos deportivos" en Google, los primeros resultados que ves son anuncios pagados por empresas que quieren que compres sus zapatos. Estas empresas pagan cada vez que alguien hace clic en su anuncio.

Pero, ¿realmente funciona? ¿Las búsquedas pagadas generan ventas adicionales, o simplemente capturan clics que de todas formas habrían llegado a la empresa a través de los resultados orgánicos (no pagados)?

Esta es una pregunta de miles de millones de dólares, y por mucho tiempo nadie la había respondido de forma rigurosa. Hasta que Thomas Blake, Chris Nosko y Steven Tadelis publicaron en 2015 su estudio sobre eBay.

eBay es una empresa tan conocida que cuando alguien busca "eBay" en Google, el resultado orgánico (no pagado) aparece como el primer resultado. A pesar de esto, eBay pagaba millones de dólares por aparecer también como anuncio pagado en las búsquedas de su propia marca.

Los investigadores convencieron a eBay de hacer un experimento. Durante un periodo, eBay dejó de pagar por publicidad en búsquedas de su propia marca en ciertos mercados, mientras que en otros mercados siguió pagando como de costumbre. Esto creó un grupo de tratamiento (sin publicidad pagada) y un grupo de control (con publicidad pagada).

Los resultados fueron reveladores: cuando eBay dejó de pagar por anuncios en búsquedas de su propia marca, los clics se sustituyeron **casi en su totalidad** por clics en los resultados orgánicos. Es decir, las personas que buscaban "eBay" en Google iban a llegar a eBay de todas formas, con o sin el anuncio pagado. eBay estaba literalmente tirando dinero a la basura.

Pero la historia tiene un matiz importante. Los investigadores también encontraron que la publicidad pagada sí tenía efecto en dos casos:

1. **Usuarios nuevos.** Las personas que no conocían eBay sí eran influenciadas por los anuncios. Para ellos, el anuncio pagado era la diferencia entre descubrir eBay o no.

2. **Marcas más pequeñas.** Para empresas que no son tan conocidas como eBay, la publicidad pagada sí puede generar ventas adicionales, porque sus resultados orgánicos no necesariamente aparecen en las primeras posiciones.

La lección de Blake et al. (2015) es doble. Primero, los experimentos pueden ahorrar mucho dinero al revelar que algo que parecía funcionar no estaba funcionando. Segundo, los resultados de un experimento no siempre son blanco o negro; los efectos pueden variar según el contexto.

## Prompt: Diseña el experimento ideal

Una herramienta útil para pensar en causalidad es pedirle a un modelo de lenguaje que te ayude a diseñar el experimento ideal para tu pregunta de investigación. Aquí hay un prompt que puedes usar:

```text
Eres un experto en inferencia causal y diseño experimental. Tu tarea es ayudarme
a diseñar el experimento ideal para responder una pregunta causal.

Mi pregunta es: [ESCRIBE TU PREGUNTA AQUÍ]

Por favor, diseña el experimento ideal siguiendo estos pasos:
1. Define claramente la variable de tratamiento y la variable de resultado.
2. Describe cómo asignarías aleatoriamente el tratamiento.
3. Identifica el grupo de control y el grupo de tratamiento.
4. Explica qué datos recolectarías y cómo los analizarías.
5. Enumera las posibles amenazas a la validez del experimento.
6. Discute si este experimento es factible en la práctica. Si no lo es, sugiere
   la mejor alternativa observacional.

Sé específico y práctico. Da ejemplos concretos.
```

Este prompt es útil incluso cuando no puedes hacer el experimento. El simple ejercicio de pensar en el diseño ideal te ayuda a clarificar qué estás tratando de medir y cuáles son los supuestos que necesitas hacer.

## Resumen del capítulo

En este capítulo exploramos el poder de los experimentos y las pruebas A/B como la herramienta más confiable para establecer relaciones causales.

Comenzamos con un ejemplo real: el experimento de publicidad en Instagram para un negocio de pestañas en Mazatlán, donde probamos 8 variantes de anuncios y descubrimos que el mejor era cinco veces más eficiente que el peor. Este ejemplo ilustra cómo los experimentos eliminan el debate y lo reemplazan con evidencia.

Vimos que los experimentos son el *gold standard* de la ciencia porque, al asignar aleatoriamente a los participantes, eliminan las variables confusoras y nos permiten atribuir las diferencias en los resultados directamente al tratamiento. En los negocios, los experimentos son especialmente valiosos porque eliminan la duda, simplifican el análisis, producen resultados interpretables y pueden ser más baratos que las alternativas.

También discutimos qué hacer cuando no se puede experimentar. La recomendación de Angrist y Pischke es siempre empezar pensando en el experimento ideal, porque esto nos ayuda a identificar los supuestos necesarios para cualquier análisis alternativo.

Reconocimos que hay preguntas que ni siquiera un experimento puede responder, como el efecto de la edad en el emprendimiento, porque ciertas variables son inseparables de otras.

Finalmente, el estudio de Blake et al. (2015) sobre eBay nos mostró cómo un experimento reveló que millones de dólares en publicidad pagada no estaban generando ventas adicionales, con la importante excepción de usuarios nuevos y marcas menos conocidas.

## Ejercicios

1. **El experimento de las pestañas (Conceptual).** En el ejemplo del negocio de pestañas, usamos $2^3 = 8$ variantes de anuncios. Si quisiéramos añadir una cuarta variable (por ejemplo, el color de fondo del anuncio: claro u oscuro), ¿cuántas variantes tendríamos que probar? ¿Por qué el número de variantes crece tan rápido y qué implicaciones tiene esto para el presupuesto del experimento?

2. **Validez interna vs. externa (Conceptual).** El experimento de eBay demostró que la publicidad pagada no generaba ventas adicionales para eBay. ¿Significa esto que la publicidad pagada en Google no funciona para ninguna empresa? Explica la diferencia entre la validez interna (¿el resultado es correcto para eBay?) y la validez externa (¿el resultado aplica a otras empresas?) del estudio de Blake et al. (2015).

3. **Diseña tu propio experimento (Práctica).** Piensa en una pregunta de negocios que te interese (puede ser de tu trabajo, de un negocio que te gustaría tener, o de una empresa que admires). Usa el prompt del capítulo para diseñar el experimento ideal. Describe: (a) la pregunta, (b) la variable de tratamiento, (c) la variable de resultado, (d) cómo asignarías el tratamiento aleatoriamente, y (e) una posible amenaza a la validez del experimento.

4. **El costo de no experimentar (Reflexión).** El capítulo menciona que el costo de oportunidad de debatir sin datos puede ser mayor que el costo de un experimento. Describe una situación (real o hipotética) en la que una empresa tomó una decisión importante basándose en opiniones en lugar de datos. ¿Cómo habría cambiado la situación si hubieran hecho un experimento?

5. **Preguntas sin respuesta (Conceptual).** El capítulo discute cómo la edad es inseparable de la experiencia, el capital y otros factores. Piensa en otra variable que sea igualmente difícil de aislar. Describe por qué un experimento no podría responder la pregunta causal asociada y qué alternativas tendrías para al menos aproximar una respuesta.

6. **eBay y los usuarios nuevos (Análisis).** Blake et al. (2015) encontraron que la publicidad pagada sí funcionaba para usuarios nuevos de eBay. ¿Por qué crees que este grupo responde de forma diferente? ¿Qué nos dice esto sobre la importancia de analizar los resultados de un experimento por subgrupos en lugar de solo mirar el efecto promedio?

7. **El mapa del tesoro (Conceptual).** El capítulo usa la metáfora de un mapa del tesoro para explicar por qué es útil pensar en el experimento ideal incluso cuando no lo puedes ejecutar. Toma una de las siguientes preguntas y describe cuál sería el experimento ideal y por qué no se puede llevar a cabo: (a) ¿El salario mínimo reduce el empleo? (b) ¿Tener un título universitario aumenta los ingresos? (c) ¿Las redes sociales causan depresión en adolescentes?

8. **Ética en los experimentos (Reflexión).** Facebook (ahora Meta) fue criticado en 2014 por un experimento en el que manipuló el *news feed* de algunos usuarios para mostrarles más contenido negativo y estudiar el efecto en sus emociones. ¿Dónde crees que está la línea entre un experimento de negocios legítimo (como una prueba A/B de un botón) y un experimento éticamente cuestionable? ¿Qué criterios usarías para decidir si un experimento es aceptable?

9. **De la teoría a la práctica (Aplicación).** Encuentra un ejemplo real de una prueba A/B publicada por una empresa (muchas empresas de tecnología publican sus resultados en blogs de ingeniería). Describe: (a) qué probaron, (b) cómo midieron el resultado, (c) qué encontraron, y (d) si crees que el diseño del experimento fue adecuado. Si no encuentras un ejemplo, puedes usar el caso del botón de "Comprar" de Amazon o cualquier caso conocido.
