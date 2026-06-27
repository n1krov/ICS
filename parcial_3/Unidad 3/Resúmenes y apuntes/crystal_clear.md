---
title: "Ingeniería y Calidad de Software"
author: "Agus, Fabri y Juani"
date: "25-06-2025"
geometry: margin=1.6in
colorlinks: true
header-includes:
  - \usepackage{fvextra}
  - \DefineVerbatimEnvironment{Highlighting}{Verbatim}{breaklines,commandchars=\\\{\}}
  - \usepackage{graphicx}
  - \setkeys{Gin}{width=0.75\textwidth}
  - \usepackage{float}
  - \floatplacement{figure}{H}
  
  # neutralizamos tightlist y ajustamos espaciado de listas
  - \let\tightlist\relax
  - \usepackage{enumitem}
  - \setlist[itemize,enumerate]{itemsep=1\baselineskip, topsep=1\baselineskip}
  
  # estilo rosado pálido con fuente aclarada
  - \usepackage[most]{tcolorbox}
  - |
    \newtcolorbox{noteBox}{
      colback=red!5!white,
      colframe=red!30!black,
      coltext=black!70,        % color del texto menos saturado
      arc=4pt,
      left=6pt, right=6pt, top=4pt, bottom=4pt,
      boxrule=0.5pt,
      breakable
    }
  - |
    \renewenvironment{quote}{\begin{noteBox}}{\end{noteBox}}
---

# Crystal Clear

Crystal Clear es una metodología de desarrollo de software diseñada por Alistair Cockburn, cuyo objetivo principal es ayudar a pequeños equipos a llevar sus proyectos a una "zona de seguridad". Se describe como una **metodología impulsada por humanos** que es simple y tolerante, con apenas los recursos necesarios para que el sistema salga adelante.

Alistair Cockburn desarrolló Crystal Clear a partir de diez años de entrevistas con equipos pequeños y exitosos, observando que muchos de ellos repetían las mismas prácticas clave.

## Alcance y propósito de Crystal Clear:

* Está diseñada para **equipos pequeños**, específicamente para un diseñador principal y entre 2 y 7 desarrolladores adicionales, ubicados en una sala grande o en habitaciones adyacentes. Es importante destacar que no está pensada para equipos más grandes ni para sistemas críticos para la vida humana sin adaptaciones adicionales.
* Prioriza la **seguridad en el resultado del proyecto**, la **eficiencia en el desarrollo** y la **habitabilidad de las convenciones** para los desarrolladores. La habitabilidad significa que las reglas deben ser aquellas con las que el equipo pueda convivir.
* Su filosofía es ser **"suficiente"** en lugar de "la mejor" metodología, permitiendo que el equipo la adapte a sus propias necesidades y, por lo tanto, la utilice realmente.

## La esencia de Crystal Clear se describe de la siguiente manera:

El diseñador principal y entre 2 y 7 desarrolladores se encuentran en una sala grande o en habitaciones adyacentes, con "radiadores de información" como pizarras blancas y rotafolios en la pared. Tienen fácil acceso a usuarios clave, se mantienen las distracciones alejadas, y **entregan código funcional, probado y utilizable cada uno o dos meses (tres meses como máximo)**. Además, periódicamente **reflexionan y ajustan su estilo de trabajo**.

## Fundamentos y principios:

Crystal Clear se basa en la caracterización del desarrollo de software como un **"juego cooperativo de invención y comunicación económicamente restringido"**. Esto implica que las personas y su capacidad de inventar y comunicarse son clave para el resultado del proyecto, y que cada decisión tiene consecuencias económicas.

### Los principios que guían Crystal Clear incluyen:

* **Las diferentes proyectos necesitan diferentes compensaciones metodológicas**.
* **Equipos más grandes necesitan más elementos de comunicación**.
* **Proyectos con mayor daño potencial necesitan más elementos de validación**.
* **Poca metodología hace mucho bien; después de eso, el peso es costoso**.
* **La formalidad, el proceso y la documentación no sustituyen la disciplina, la habilidad y la comprensión**.
* **La comunicación interactiva y cara a cara es el canal más barato y rápido para intercambiar información**.
* **El aumento de la retroalimentación y la comunicación reduce la necesidad de entregables intermedios**.
* **El desarrollo concurrente y en serie intercambia costo de desarrollo por velocidad y flexibilidad**.
* **La eficiencia es prescindible en actividades no-cuello de botella**.
* **Los "puntos óptimos" aceleran el desarrollo**, refiriéndose a tener personas dedicadas y experimentadas, pruebas automatizadas, acceso a usuarios expertos y entregas frecuentes.

## Las Siete Propiedades de Proyectos de Software Efectivos:

"Hacer Crystal Clear" significa lograr estas propiedades más que seguir un conjunto rígido de procedimientos. Las primeras tres son obligatorias para Crystal Clear, y las otras cuatro ayudan a llevar al equipo más lejos en la zona de seguridad.

### 1.  Entregas Frecuentes (Frequent Delivery)

La propiedad más importante de cualquier proyecto. Implica entregar código funcional y probado a usuarios reales cada pocos meses. Las ventajas son numerosas, como la retroalimentación crítica sobre el progreso y la oportunidad para que los usuarios descubran si lo solicitado originalmente era lo que realmente necesitaban. La integración frecuente (varias veces al día) es la norma, pero la "entrega" se refiere a dar el software a los usuarios, no solo a la iteración interna. Incumplir esto, como no entregar nada en casi un año a pesar de las iteraciones, es una violación.

### 2.  Mejora Reflexiva (Reflective Improvement)

La capacidad de un proyecto para revertir su situación, incluso de un fracaso catastrófico a un éxito, si el equipo se reúne, lista lo que funciona y lo que no, discute qué podría funcionar mejor y aplica esos cambios en la siguiente iteración. Se sugiere una reunión de una hora cada pocas semanas o al mes.

### 3.  Comunicación Osmótica (Osmotic Communication)

Significa que la información fluye al oído de los miembros del equipo en segundo plano, permitiéndoles captar información relevante como por ósmosis. Se logra normalmente sentando a los miembros del equipo en la misma sala, donde las preguntas y respuestas fluyen naturalmente con poca interrupción. Esto permite una retroalimentación rápida y rica, reduciendo la necesidad de mucha otra estructura. La separación física, incluso por un pasillo o una puerta con seguro, afecta negativamente esta comunicación.

### 4.  Seguridad Personal (Personal Safety)

La capacidad de expresar lo que a uno le molesta sin temor a represalias, lo cual es crucial para que el equipo descubra y repare sus debilidades. Es un paso temprano hacia la confianza.

### 5.  Enfoque (Focus)

Saber en qué trabajar y tener el tiempo y la tranquilidad para hacerlo. El patrocinador ejecutivo es quien aclara las prioridades de lo que tiene valor para el negocio. Se recomienda garantizar al menos dos días consecutivos y dos horas ininterrumpidas cada día para el trabajo.

### 6.  Fácil Acceso a Usuarios Expertos (Easy Access to Expert Users)

El acceso continuo a usuarios expertos proporciona al equipo un lugar para desplegar y probar las entregas frecuentes, retroalimentación rápida sobre la calidad del producto y las decisiones de diseño, y requisitos actualizados. Incluso una hora a la semana de acceso es inmensamente valiosa.

### 7.  Entorno Técnico con Pruebas Automatizadas, Gestión de Configuración e Integración Frecuente

Estos son elementos fundamentales. Las pruebas automatizadas, aunque no son un factor crítico de éxito, ofrecen velocidad y seguridad. La gestión de configuración es una de las herramientas más importantes. La integración debe ser frecuente (varias veces al día, al menos dos veces por semana).

## Prácticas y recomendaciones clave:

* **Colocación**: Sentar a la gente muy cerca para facilitar la comunicación osmótica. Un "war room" es lo ideal, o al menos oficinas adyacentes que permitan oír las conversaciones.
* **Usuario Real Directamente Involucrado**: Un usuario experto debe estar disponible para el equipo, incluso si es a tiempo parcial, para revisar el sistema y validar diseños.
* **Pruebas Automatizadas de Regresión**: Diseñar una arquitectura que soporte pruebas de regresión totalmente automatizadas. Esto da libertad para hacer cambios y una sensación de seguridad.
* **Funcionalidad Entregable Temprano y Frecuentemente**: Producir y entregar código funcional en periodos cortos.
* **Pizarras Blancas como Medio de Diseño Primario**: Utilizar pizarras para el diseño y la documentación, incluso fotografiándolas para el registro.
* **"Peer Code Peering" o Programación Lado a Lado**: Examinar y comentar pequeñas cantidades de código de forma continua, facilitado por la proximidad física.
* **Rol del Diseñador Principal**: Se espera que el diseñador principal sea un desarrollador de "Nivel 3" (fluidez), capaz de ajustar el proceso sobre la marcha y entender las propiedades deseadas del proyecto.
* **Gestión de Configuración**: La herramienta de gestión de configuración es una de las herramientas más importantes mencionadas por casi todos los equipos exitosos.
* **"Walking Skeleton" (Esqueleto Andante)**: Una implementación mínima del sistema que realiza una función completa de principio a fin, conectando los componentes arquitectónicos principales. Es código permanente y probado, que crece con el sistema.
* **"Information Radiators" (Radiadores de Información)**: Pantallas (pizarras, rotafolios, monitores) colocadas donde las personas puedan verlas mientras trabajan o pasan, mostrando información relevante sin necesidad de preguntar.
* **Reuniones Diarias de Pie (Daily Stand-Up Meetings)**: Reuniones cortas donde cada persona responde qué hizo ayer, qué planea hacer hoy y qué se interpone en su camino. Son muy efectivas para difundir información y mantener el enfoque.
* **Metodología es Convenios del Equipo**: La metodología es simplemente el conjunto de convenciones que el equipo acuerda adoptar. Estas convenciones deben revisarse y ajustarse periódicamente.

## Tolerancia y flexibilidad:

Crystal Clear es una metodología de alta tolerancia. Permite al equipo decidir sobre el estilo de codificación, las herramientas específicas, la duración de las iteraciones (rango de 1 a 3 meses para la entrega) y el tipo de documentación intermedia. No exige ninguna técnica o herramienta específica. Se espera que los equipos tomen prestadas ideas de otras metodologías (como Scrum o XP). La documentación es necesaria, pero su forma y cantidad deben ser decididas por el equipo en conjunto con el patrocinador, buscando un equilibrio entre el progreso a corto plazo y la necesidad de información para futuros mantenimientos.

## En resumen

Crystal Clear se centra en empoderar a equipos pequeños y ubicados en el mismo lugar, confiando en su comunicación y capacidad de autoajuste para entregar software de valor de manera eficiente y sostenible, priorizando la seguridad y la habitabilidad sobre la rigidez de los procesos.

---
