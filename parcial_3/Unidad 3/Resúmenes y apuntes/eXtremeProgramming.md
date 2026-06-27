---
title: "Resumen: eXtreme Programming"
author: "Juani y Kent Beck"
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

Extreme Programming (XP) es una **metodología ligera de desarrollo de software** que fue concebida y desarrollada para abordar las necesidades específicas de equipos pequeños que trabajan con **requisitos vagos y cambiantes**. Se la considera "extrema" porque toma principios de sentido común y los lleva a niveles muy altos.

# **Aspectos Fundamentales y Características Clave de XP**

* **Enfoque en el Cambio y el Riesgo**: XP reconoce que el costo de cambiar una pieza de software no necesariamente aumenta drásticamente con el tiempo. Se basa en la premisa de que esta curva de costos puede aplanarse a través de una combinación de tecnología y prácticas de programación. Esto permite que el proyecto se adapte continuamente a los cambios en los requisitos y el entorno empresarial, lo que reduce el riesgo del proyecto y mejora la capacidad de respuesta a los cambios de negocio.
* **Filosofía de la Suficiencia**: XP es un experimento que pregunta: "¿Cómo programarías si tuvieras suficiente tiempo?". Esto fomenta una mentalidad que valora escribir pruebas, reestructurar el sistema a medida que se aprende y mantener una comunicación constante, en contraste con la mentalidad de escasez que a menudo genera desperdicio.

## **Cuatro Valores Centrales**

Estos valores guían el éxito del equipo y su estilo de desarrollo:

* **Comunicación**: Es fundamental para el éxito del proyecto, ya que la mayoría de los problemas se remontan a la falta de diálogo. XP emplea prácticas que exigen comunicación constante, como las pruebas unitarias, la programación en pares y la estimación de tareas.
* **Simplicidad**: Se busca la "cosa más simple que pueda funcionar" en cualquier momento. Esto significa hacer lo simple hoy, incluso si se requiere un pequeño costo adicional para cambiarlo mañana, en lugar de implementar una solución compleja que podría no usarse.
* **Retroalimentación (Feedback)**: Se obtiene retroalimentación concreta y continua sobre el estado del sistema en diferentes escalas de tiempo (minutos, días, semanas, meses). Esto incluye pruebas unitarias, pruebas funcionales del cliente y revisiones de cronograma. La retroalimentación es clave para el aprendizaje y la mejora.
* **Coraje**: Es necesario para tomar decisiones difíciles, como tirar código si es necesario, refactorizar el sistema o experimentar con nuevas ideas. El coraje se apoya en los otros tres valores.
* Un valor subyacente es el **Respeto** entre los miembros del equipo y por el proyecto.

## **Principios Básicos** 

Derivados de los **valores**, incluyen:

* Retroalimentación rápida.
* Asumir simplicidad.
* Cambio incremental.
* Abrazar el cambio.
* Trabajo de calidad.
* Otros principios menos centrales pero importantes son enseñar el aprendizaje, pequeña inversión inicial, jugar para ganar, experimentos concretos, comunicación abierta y honesta, trabajar con los instintos de las personas, responsabilidad aceptada, adaptación local, viajar ligero y medición honesta.

## **Cuatro Actividades Básicas de Desarrollo**

XP estructura las cuatro actividades esenciales del desarrollo de software:

* **Codificación**: El resultado final de todo el proceso. Es la mejor manera de aprender y comunicar ideas, y es el artefacto que el desarrollo no puede prescindir.
* **Pruebas**: Las pruebas automatizadas son fundamentales; las funcionalidades sin una prueba automatizada "simplemente no existen". Los programadores escriben pruebas unitarias y los clientes escriben pruebas funcionales. Las pruebas dan confianza y reducen el tiempo de depuración.
* **Escucha**: Los programadores deben escuchar activamente a los clientes para entender los problemas de negocio y obtener los requisitos necesarios para las pruebas.
* **Diseño**: Se refiere a la creación y evolución continua de la estructura del sistema para organizar la lógica de manera efectiva. El diseño en XP se refina continuamente a partir de un inicio muy simple, eliminando la flexibilidad que no resulta útil.

# **Las Prácticas Clave de XP**

Las prácticas de XP trabajan en conjunto, y las debilidades de una práctica suelen ser compensadas por las fortalezas de otras.

* **El Juego de Planificación (The Planning Game)**: Determina el alcance de la próxima entrega combinando las prioridades de negocio y las estimaciones técnicas. El negocio decide el alcance, la prioridad, la composición y las fechas de las entregas, mientras que el equipo de desarrollo proporciona estimaciones y organiza el trabajo.
* **Entregas Pequeñas (Small Releases)**: Un sistema simple se pone en producción rápidamente, con nuevas versiones lanzadas en ciclos muy cortos (desde diarios hasta bimensuales).
* **Metáfora (Metaphor)**: Una historia simple y compartida que guía todo el desarrollo y ayuda a todos a entender los elementos básicos del sistema y sus relaciones. Reemplaza gran parte de lo que otros llaman "arquitectura".
* **Diseño Simple (Simple Design)**: El sistema debe tener el diseño más simple posible que cumpla con todos los tests, no contenga lógica duplicada, exprese las intenciones de los programadores y tenga el menor número de clases y métodos posible.
* **Pruebas (Testing)**: Los programadores escriben continuamente pruebas unitarias que deben ejecutarse sin fallos. Los clientes escriben pruebas funcionales que demuestran que las funcionalidades están terminadas.
* **Refactorización (Refactoring)**: Los programadores reestructuran el sistema sin cambiar su comportamiento para eliminar duplicaciones, mejorar la comunicación, simplificar o añadir flexibilidad.
* **Programación en Parejas (Pair Programming)**: Todo el código de producción se escribe con dos programadores en una misma máquina. Uno se enfoca en la implementación detallada, mientras el otro piensa más estratégicamente. Fomenta la comunicación y mejora la calidad del código.
* **Propiedad Colectiva (Collective Ownership)**: Cualquier miembro del equipo puede cambiar cualquier código en cualquier parte del sistema en cualquier momento si ve una oportunidad de mejora.
* **Integración Continua (Continuous Integration)**: El código se integra y prueba varias veces al día, después de que se completa cada tarea. Esto reduce el riesgo del proyecto y la complejidad de las fusiones.
* **Semana de 40 Horas (40-Hour Week)**: Se fomenta trabajar un máximo de 40 horas a la semana y nunca trabajar horas extras dos semanas seguidas para mantener al equipo fresco y creativo.
* **Cliente en Sitio (On-Site Customer)**: Un usuario real del sistema se incluye en el equipo, disponible a tiempo completo para responder preguntas, resolver disputas y establecer prioridades a pequeña escala.
* **Estándares de Codificación (Coding Standards)**: Los programadores escriben todo el código siguiendo reglas que enfatizan la comunicación a través del código.

# **La Economía del Desarrollo de Software en XP**

XP busca maximizar el valor económico de un proyecto de software al **gastar dinero más lentamente, generar ingresos más rápidamente y aumentar la vida útil productiva** del proyecto. Considera la gestión de proyectos como una serie de opciones (abandonar, cambiar, diferir, crecer), siendo el valor de estas opciones dominado por la incertidumbre. Por lo tanto, XP es especialmente valioso cuando los requisitos son **vagos o cambiantes**.

# **Ciclo de Vida de un Proyecto XP Ideal**

Un proyecto XP ideal pasa por fases de:

* **Exploración**: Fase inicial donde el cliente y los programadores determinan las posibilidades del sistema y la viabilidad tecnológica.
* **Planificación**: El cliente y los programadores acuerdan una fecha para la primera entrega y el conjunto de historias más valiosas a implementar.
* **Iteraciones hasta la Primera Entrega**: Ciclos de una a cuatro semanas donde se implementan historias y se realiza un seguimiento constante del progreso.
* **Puesta en Producción (Productionizing)**: Fase de preparación para el lanzamiento, donde se ajustan los ciclos de retroalimentación y se realizan pruebas adicionales.
* **Mantenimiento**: El estado normal de un proyecto XP, donde se produce nueva funcionalidad y se mantiene el sistema existente.
* **Muerte**: La retirada planificada y consciente del sistema cuando ya no es viable económicamente o no se necesitan más funcionalidades.

# **Roles en un Equipo XP**

Aunque los roles son flexibles, algunos son fundamentales:

* **Programador**: Es el corazón de XP, encargado de analizar, diseñar, probar, programar e integrar.
* **Cliente**: Sabe qué programar, escribe historias, define pruebas funcionales y toma decisiones de prioridad y alcance.
* **Tester**: Ayuda al cliente a escribir y ejecutar pruebas funcionales, y asegura que las herramientas de prueba funcionen.
* **Tracker**: Mide el progreso del proyecto, recopila métricas y proporciona retroalimentación sobre las estimaciones del equipo.
* **Coach**: Es responsable del proceso general, observa las desviaciones y guía al equipo de forma indirecta.
* **Consultor**: Proporciona conocimiento técnico especializado al equipo cuando es necesario, trabajando de cerca con los programadores para transferir conocimientos.
* **Big Boss**: Proporciona coraje, confianza y asegura que el equipo cumpla con sus compromisos, aceptando la comunicación honesta sobre el progreso.

# **Cuándo NO Usar XP**

XP no es adecuado para todos los proyectos o entornos. Algunas situaciones donde XP puede fallar incluyen:

* **Equipos muy grandes**: No funciona bien con cientos, cincuenta o incluso veinte programadores.
* **Clientes desconfiados**: Requiere una relación de confianza y voluntad de diálogo continuo con el cliente.
* **Tecnología inflexible**: Si se usa una tecnología con un costo de cambio inherentemente exponencial o un entorno donde la retroalimentación es muy lenta (ej., compilaciones de 24 horas, ciclos de QA de dos meses).
* **Ambiente físico inadecuado**: Un espacio de trabajo abierto y colaborativo es crucial; si los programadores están dispersos o el ruido impide la comunicación, XP no alcanzará su máximo potencial.
* **Cultura empresarial opuesta**: Si la cultura de la empresa insiste en especificaciones rígidas, planes detallados por adelantado o largas horas de trabajo para demostrar "compromiso".

# **Dificultades de XP**

Aunque simple en sus detalles, XP es **difícil de ejecutar**. La principal dificultad reside en las **emociones, especialmente el miedo**:

* Es difícil hacer cosas simples cuando se ha tenido éxito con lo complicado.
* Es difícil admitir no saber.
* Es difícil colaborar, ya que los sistemas educativos y de recompensa suelen enfocarse en el logro individual.
* Es difícil derribar muros emocionales y comunicar abiertamente frustraciones o miedos.
* Los pequeños problemas en el proceso pueden tener efectos enormes.

A pesar de sus desafíos, XP promete **reducir el riesgo del proyecto, mejorar la capacidad de respuesta a los cambios de negocio, aumentar la productividad y añadir diversión** al desarrollo de software en equipo.
