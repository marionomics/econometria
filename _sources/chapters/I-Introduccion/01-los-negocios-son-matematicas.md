# Los negocios son matemáticas

> *Es mejor haber entendido por qué fallaste que ser ignorante de por qué tuviste éxito*
>
> \- Robert A. Burgelman

**Cuando salí de la universidad**, tenía un solo objetivo: abrir mi propio negocio. Había emprendido de muchas formas durante la carrera: había vendido promociones para una taquería que comenzamos en mi familia (falló) y había aprendido a crear productos que solucionan problemas y sabía vender. Ya estaba listo para las grandes ligas (según yo).

El año era 2009: justo en medio de la gran recesión.

La gran recesión afectó los ingresos de mi generación de una manera brutal. Quienes salimos al mundo laboral ese año nos encontramos un escenario post-apocalíptico sin opciones de trabajo y con negocios cerrando por doquier.

Y fue en los negocios que cerraban donde vi oportunidad (no hagas esto en casa).

Mi café favorito estaba en venta. Era un café en el centro histórico, con una clientela establecida y operando al 100%. Era la oportunidad perfecta para poner en práctica todo lo que había aprendido los últimos cuatro años en la universidad (o eso creía yo).

El único problema era que no tenía dinero.

Decidí juntar 10 amigos, hacerlos socios y comprar el negocio. Venía junto con una renta mensual de 11 mil pesos y un barista muy hábil, aunque un poco antipático. Hice modificaciones mínimas y abrimos al público ese mismo mes. Jamás olvidaré la sensación de abrir un negocio y comenzar a recibir clientes ese mismo día. Pensé que si seguía a ese mismo ritmo, recuperaría mi inversión en menos de un mes y me imaginaba como el próximo Steve Jobs antes de los 30.

Para noviembre de ese mismo año, acabé con una neumonía que casi me mata y el negocio quebrado.

## Cometí dos errores grandes con ese negocio

Si no hubiera cometido estos errores, habría tenido un negocio exitoso en lugar del rotundo fracaso que viví.

- **El primer error fue no haberme ensuciado las manos lo suficiente.** Pensaba que mis conocimientos de administración eran suficientes para manejar cualquier situación. Si volviera al pasado, habría dedicado más tiempo a aprender a hacer todo en la operación del negocio. ¡Al menos hubiera aprendido a hacerla de barista!
- **Mi segundo error fue seguir demasiado mi intuición y muy poco a lo que decían los datos.** También fue por arrogancia. Saliendo de la universidad sentía que ya lo sabía todo y que todos los demás estaban equivocados.

Nunca más.

## Usar datos en los negocios significa tener la humildad de aceptar que no lo sabemos todo

En retrospectiva, veo que no fue una idea absurda. No estaba loco, simplemente no entendí los números.

```{figure} ../../figures/intro/gdp.png
---
name: fig-gdp-mexico
---
Crecimiento del PIB de México de 1990 a la actualidad. Como millenial, me ha tocado vivir 3 crisis: la crisis del peso mexicano (o efecto tequila), la llamada "gran recesión" y la crisis del Covid-19. Fuente: Elaboración propia con datos del Banco Mundial.
```

Para convencer a 10 amigos a que invirtieran conmigo usé gráficas del ciclo económico. Les expliqué que probablemente estábamos en el punto más bajo y que la economía no tenía más opción que subir. Los datos históricos me respaldaban, pero esta no era una recesión normal, sino una crisis financiera con raíces estructurales profundas.

Si hubiera sido más cuidadoso al revisar los datos, probablemente no habría tomado un riesgo tan alocado.

## Este libro está diseñado para un mundo donde la Inteligencia Artificial puede hacer análisis de datos

La primera sección se enfoca en el mindset de la inferencia causal.

Hoy en día ya es posible subir una base de datos a ChatGPT y pedirle que limpie y prepare los datos para hacer análisis. Luego le puedes pedir que haga una regresión lineal y que te dé su interpretación de los resultados. Finalmente, le puedes pedir que haga las pruebas de hipótesis más comunes.

Pero incluso con todo eso, hay algo que la IA todavía no puede hacer: distinguir entre correlación y causalidad. Eso sólo lo vas a poder hacer tú. Porque eres tú el que tiene una *ventana de contexto* más completa (la ventana de contexto es el número de tokens que una IA usa en su memoria para dar respuestas; todos los días aumenta más, pero la forma en que los humanos damos contexto y conectamos ideas lo considero más potente), tienes ojos y oídos y puedes salir al mundo a ver si tus hipótesis tienen sentido o no.

La segunda sección tiene elementos de negocios indispensables para generar crecimiento basado en datos.

El análisis de datos hoy en día es un elemento integral de los negocios. No se trata de un accesorio adicional: los datos son tu negocio. Cada paso que damos en negocios, lo debemos hacer tomando la evidencia como un elemento central.

En la última sección veremos los modelos más avanzados. Porque al inicio estaremos intentando hacer experimentos, pero cuando no es posible hacer uno, nos apoyaremos en los llamados **experimentos naturales** para hacer modelos de diferencias en diferencias que nos entreguen resultados con interpretación similar a la que tendríamos si hiciéramos un experimento.

> *It's the economist way.*

## ¿Qué necesitas saber antes de comenzar?

Lo más importante son tus ánimos de aprender y tu curiosidad.

Procuro a lo largo de este libro mantener las ideas a nivel intuitivo. Sin embargo, hay algunos temas que requieren conocimientos previos:

- En el capítulo de Regresión, cuando paso de la regresión con una variable a múltiples variables, explico el resultado final usando álgebra lineal. Es un segmento que te puedes saltar, pero me pareció indispensable explicarlo de esa manera.
- En general, a lo largo del libro, usamos modelos sencillos, pero es necesario tener una intuición sobre lo que representa una variable aleatoria y cómo funciona la probabilidad básica.
- Comenzamos el libro con un repaso de programación en Python. Aunque es muy básico, es suficiente para entender el código en los siguientes capítulos o al menos formar una intuición. Sin embargo, te recomiendo hacer más ejercicios para solidificar tu conocimiento.

## Resumen

En este capítulo introductorio compartí la historia de mi primer negocio fallido para ilustrar la importancia de usar datos en la toma de decisiones. Los dos errores principales fueron: no involucrarme lo suficiente en la operación y confiar demasiado en la intuición en lugar de analizar los datos con rigor. Este libro está diseñado para un mundo donde la IA puede hacer análisis de datos, pero donde la capacidad de distinguir entre correlación y causalidad sigue siendo una habilidad humana fundamental.

## Ejercicios

1. Piensa en una decisión importante que hayas tomado basándote en tu intuición. ¿Qué datos podrías haber consultado antes de tomarla?

2. Busca un ejemplo reciente en las noticias donde se confunda correlación con causalidad. Describe el ejemplo y explica por qué la conclusión podría ser incorrecta.

3. Investiga brevemente qué fue la "gran recesión" de 2008-2009. ¿Qué indicadores económicos habrías revisado antes de invertir en un negocio en ese momento?

4. ¿Cuál es la diferencia entre correlación y causalidad? Escribe un ejemplo de cada una con tus propias palabras.

5. Imagina que tienes un negocio de comida y las ventas bajan un 20% en un mes. Haz una lista de al menos 5 posibles causas y describe qué datos buscarías para investigar cada una.

6. Reflexiona sobre el concepto de "ventana de contexto" que se menciona en el capítulo. ¿Por qué crees que los humanos todavía tenemos una ventaja sobre la IA al momento de interpretar datos?

7. Describe un escenario en el que un experimento natural podría ayudarte a entender el efecto de una política pública. ¿Qué datos necesitarías?

8. Lee sobre el ciclo económico y dibuja una gráfica simplificada. Marca en qué punto del ciclo crees que estamos actualmente y justifica tu respuesta con al menos un dato o indicador.
