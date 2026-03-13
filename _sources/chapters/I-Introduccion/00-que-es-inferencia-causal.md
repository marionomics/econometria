# Antes de comenzar: ¿Qué es la inferencia causal?

A mediados del siglo XIX hubo un brote de cólera que cambió el mundo por completo (John Snow luego le llamaría "El brote más terrible de cólera que haya ocurrido en este reino").

El cólera es una enfermedad terrible. Hoy en día sabemos con certeza que su origen proviene de una bacteria. Saber esto es muy útil: si nos llegara a infectar esa bacteria, simplemente tendríamos que tomar un antibiótico y asunto resuelto. Nuestra vida no estaría en peligro.

Pero para las personas que vivían en Londres en 1854, saber la verdad era cuestión de vida o muerte.

A lo largo de la historia hubo muchas pandemias de cólera. La primera registrada es la de 1817 a 1824 y desde entonces la Organización Mundial de la Salud (OMS) considera siete pandemias distintas. Aunque las pandemias son eventos separados, algunas se han extendido por décadas, como la que comenzó en 1961 y sigue vigente hasta el día de hoy. El brote de 1854 de Londres sucedió en la calle Broad Street y mató a 616 personas.

## En la época, la teoría dominante de la causa del cólera era el *miasma*

```{figure} ../../figures/antes/pump.png
---
width: 100%
name: fig-pump
---
Broad Street en Londres durante el brote de cólera de 1854. John Snow apunta a la bomba de agua como fuente de la enfermedad. Fuente: imaginado por el autor y creado por DALL-E 3.
```

El *miasma* se refería a **aires malos**. La idea era que las enfermedades se transmitían por los aires de una persona enferma. Es una teoría que duró por muchos siglos desde Hipócrates, más de 400 años antes de Cristo hasta que la teoría de los gérmenes la sustituyó (fue hasta los 1860s que Louis Pasteur publicó su trabajo).

John Snow aún no sabía de la teoría de los gérmenes, pero no le convencía la teoría del *miasma* y decidió ponerla a prueba.

Usó lo que los economistas conocemos como un experimento natural.

```{note}
Un *experimento natural* ocurre cuando las condiciones del mundo real imitan un experimento aleatorio. Veremos más al respecto más adelante.
```

En la zona de la epidemia habían dos compañías que tomaban el agua del río Támesis y la distribuían en la ciudad: *Southwark and Vauxhall* y *Lambeth*. El agua que llevaban estaba muy contaminada. **Visiblemente** contaminada. Fue durante el mismo periodo que Lambeth decidió cambiar su toma de agua un poco más río arriba.

```{note}
El problema era que todos los desechos de la ciudad desembocaban en el río Támesis. Entre esos deshechos, naturalmente, estaban las heces de todos los habitantes de una ciudad. El problema llegó a ser tan grande que en el verano de 1858 el olor insoportable obligó a los miembros del parlamento a abandonar el palacio de Buckingham en un episodio que se conoció como *el gran hedor*. Incidentalmente, fue esta la razón que motivó al parlamento a cambiar el sistema de drenaje de la ciudad.
```

La gran aportación de John Snow fue haber tomado nota de las muertes por cólera antes y después del cambio de la toma de agua. El cuadro muestra este registro para las dos empresas. Snow notó que algunos distritos recibían su agua de ambas compañías, pero otros tomaban su agua de una compañía en específico.

Esta era la clave para identificar sin lugar a dudas que la causa de la enfermedad era el agua y no los malos aires.

Observa las muertes por cólera de los distritos donde el suministro de agua es Southwark & Vauxhall. Prácticamente no hay cambio. En cambio, pon atención a las muertes por cólera de los distritos que suministraban su agua de Lambeth: cayeron dramáticamente. Las muertes de los distritos que se suministraban de ambas compañías también cayeron, pero ese dato no sería tan informativo sin los datos por separado.

| **Suministro de Agua** | **Muertes en 1849** | **Muertes en 1854** |
|---|---|---|
| Lambeth | 162 | 37 |
| Southwark & Vauxhall | 2261 | 2458 |
| Lambeth y Southwark & Vauxhall | 3905 | 2547 |

*Tabla de resumen de las muertes antes y después del cambio de la toma de agua por la compañía Lambeth. Fuente: Elaboración propia basada en Snow (1859), p. 90.*

## La inferencia causal se trata más de sentido común que de la estadística en sí misma

Más de 150 años después, el desafío sigue siendo similar. Hoy en día tenemos mucha más disponibilidad de datos que en 1859, y a pesar de eso, estamos en el punto en el que somos más vulnerables a la desinformación.

Durante la pandemia de Covid-19, la desinformación fue responsable de la muerte de muchas personas. Un estudio demostró que en Estados Unidos, las personas afiliadas al partido Republicano fueron más vulnerables a las noticias falsas sobre los efectos de las vacunas. La consecuencia fue que hubo un exceso de muertes 43% mayor entre republicanos que entre demócratas.

El problema es que estamos tan inundados ahora con información, que lo más crítico es saber qué hacer con ella.

John Snow reunió muchos datos sobre las muertes por cólera. Pero su contribución más importante fue darle sentido a esos datos para transformarlos en información. No se limitó a recolectar datos: él entendía la importancia de explicar las causas y efectos y comunicarlos correctamente.

Esa es la esencia de la inferencia causal.

```{figure} ../../figures/antes/snow.jpg
---
width: 100%
name: fig-snow-map
---
El mapa que John Snow trazó para identificar que el origen del cólera no era el *miasma*, sino el agua contaminada. Ubicar geográficamente los brotes en un mapa es algo que no se había hecho antes y ayudó a identificar con facilidad que la fuente era una bomba específica. Cerrar esa bomba de agua logró salvar algunas vidas, pero el modelo de pensamiento de Snow sigue salvando muchas vidas más hasta la fecha.
```

## Resumen del capítulo

En este primer capítulo viajamos en el tiempo al Londres de 1854 para conocer a John Snow, el que podría ser el primer detective de datos de la historia, y su lucha contra el cólera.

Lo que hicimos fue usar su historia para entender la idea más importante de este libro. Vimos cómo Snow desafió una teoría dominante pero incorrecta (el miasma) no con opiniones, sino con un método brillante. Usó un experimento natural --el hecho de que una compañía de agua cambiara su fuente mientras otra no-- para crear una comparación justa y demostrar sin lugar a dudas que la verdadera causa de la epidemia era el agua contaminada.

Esto es importante porque la historia de John Snow es la historia de origen de la inferencia causal. Nos enseña la lección fundamental: para encontrar la verdad, no basta con tener datos; necesitas un diseño de comparación inteligente. Sin un grupo de control creíble (la compañía que no cambió su agua), la evidencia de Snow habría sido solo una correlación interesante. Esta idea de buscar comparaciones justas para aislar la causa real es la base de todo lo que haremos en este libro.

¿Cómo te ayuda esto? Este capítulo te instala un nuevo software en el cerebro. De ahora en adelante, cuando escuches que "A causó B", tu primera pregunta no será sobre la estadística, sino sobre el método: "¿Con qué lo compararon?". Te da el superpoder del escepticismo estructurado. Te enseña a pensar como un detective, buscando siempre el grupo de control o el "experimento natural" escondido en los datos para poder aislar la verdadera causa. Es la base para no caer en la desinformación y para empezar a construir argumentos sólidos.

## Conviértete en un detective de datos: ejercicios introductorios

La inferencia causal empieza con la forma en que piensas. Estos ejercicios son para que practiques la lógica de detective que usó John Snow.

1. **El Miasma Moderno (Conceptual):** La teoría del miasma era una explicación fácil pero incorrecta. Piensa en un "miasma moderno": una correlación que la gente comúnmente confunde con una causa. (Ejemplo: "Las empresas que más invierten en publicidad en el Super Bowl son las más exitosas"). ¿Por qué esta afirmación podría ser una correlación y no una causa directa?

2. **El Grupo de Control es tu Ancla (Conceptual):** Imagina que John Snow solo hubiera tenido los datos de la compañía Lambeth (la que mejoró su agua). Habría visto que las muertes bajaron y podría haber dicho que esa era la prueba. ¿Por qué su argumento habría sido mucho más débil sin los datos de la compañía Southwark & Vauxhall? ¿Qué otras explicaciones para la caída de las muertes no podría haber descartado?

3. **Diseñando una Comparación Justa (Conceptual):** Quieres saber si una nueva estrategia de descuentos (tratamiento) realmente aumenta el valor promedio de compra en tu tienda en línea. Usando la lógica de John Snow, ¿cuál sería un buen "grupo de control"? ¿Por qué comparar las ventas de esta semana (con descuentos) con las de la semana pasada (sin descuentos) podría ser una comparación injusta?

4. **Encontrando Experimentos Naturales (Conceptual):** Un experimento natural ocurre cuando el mundo te "asigna" por accidente un grupo de tratamiento y uno de control. Describe un posible experimento natural que podrías usar para estudiar el efecto de:
   - a) El trabajo remoto en los precios de las rentas de oficinas. (Pista: piensa en una gran empresa que anuncia el teletrabajo permanente, afectando una zona de la ciudad más que otras).
   - b) Una nueva ciclovía en el número de accidentes viales. (Pista: la ciclovía se construye en una avenida principal, pero no en otra avenida paralela muy similar).

5. **Una Imagen Vale Más que Mil Números (Conceptual):** El capítulo dice que Snow no solo recolectó datos, sino que los comunicó correctamente. Además de su famosa tabla, ¿qué otra herramienta (visual) usó para que su argumento fuera tan convincente, y por qué crees que fue tan efectiva?

6. **Sentido Común y Estadística (Reflexión):** La frase clave del capítulo es "La inferencia causal se trata más de sentido común que de la estadística en sí misma". ¿Significa esto que las matemáticas no son importantes? ¿O que el diseño del estudio es la base sobre la cual se construye cualquier análisis estadístico? Justifica tu respuesta usando el caso de John Snow.

7. **El Universo Contrafactual (Conceptual):** Para una familia que vivía en un distrito servido por Lambeth, el "resultado contrafactual" es lo que les *hubiera* pasado si Lambeth *no hubiera* cambiado su fuente de agua. ¿Cómo usó John Snow los datos de la compañía Southwark & Vauxhall como una ventana a ese universo contrafactual?

8. **Aplicando la Lógica al Negocio (Conceptual):** El director de una cadena de cafeterías observa que las sucursales que tienen más de 10 empleados tienen mayores ventas. Propone como política que todas las sucursales contraten hasta tener al menos 10 empleados para aumentar las ventas. Como analista de datos inspirado en John Snow, ¿qué preguntas harías antes de apoyar esa decisión? ¿Qué datos buscarías para determinar si la relación es causal o solo una correlación?
