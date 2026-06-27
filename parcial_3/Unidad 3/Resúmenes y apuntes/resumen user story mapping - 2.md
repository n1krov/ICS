---
title: "Ingeniería y Calidad de Software"
author: "Juani"
date: "20-06-2025"
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

# Resumen: Capítulo 1, "The Big Picture"

El Capítulo 1, "The Big Picture" (La perspectiva general), aborda la frustración común de los equipos ágiles que, a pesar de ver progreso continuo, sienten que **han perdido la visión global de su producto**. La solución propuesta para este problema es el **mapeo de historias** (story mapping).

Aquí están las ideas principales del capítulo:

*   **El verdadero objetivo de las historias y el desarrollo de productos**: El propósito de usar historias **no es escribir mejores historias**, ni el objetivo del desarrollo de productos es solo hacer productos. En realidad, el objetivo es **construir un entendimiento compartido**. Esto se logra mediante la **colaboración con palabras e imágenes**, no solo a través de documentos escritos que pueden ser malinterpretados, como en el juego del "teléfono descompuesto". **"Los documentos compartidos no son entendimiento compartido"**.
*   **La "Tragedia del Backlog Plano"**: El capítulo ilustra este problema con el caso de Gary Levitt y su producto Mad Mimi. Gary había priorizado una lista de características (un "backlog" plano), pero el software resultante no se alineaba con su visión completa y se estaba quedando sin dinero antes de alcanzarla. Esto demuestra cómo **una simple lista priorizada puede hacer perder la visión de conjunto**.
*   **"Talk and Doc" (Hablar y documentar)**: Para evitar que las ideas se "vaporicen" durante las conversaciones, es crucial **escribirlas en tarjetas o notas adhesivas**. Esto ayuda a externalizar el pensamiento, permite recordar, reorganizar ideas y facilita la comunicación y el enfoque.
*   **Enmarcar la idea del producto**: Antes de sumergirse en los detalles, es fundamental **entender el negocio y los objetivos**. Esto incluye identificar:
    *   La gran idea.
    *   Quiénes son los clientes y usuarios y por qué lo querrían (qué problemas resuelve, qué beneficios obtendrán).
    *   Por qué la organización lo está construyendo (cómo ayuda a la empresa).
    Esto se alinea con el modelo **"ahora y después"**, que busca comprender los **resultados (outcomes)** deseados, no solo el producto (output).
*   **Describir clientes y usuarios**: Al iniciar el mapeo, se identifican los diferentes tipos de usuarios y clientes. La meta es **minimizar la cantidad de software a construir**, enfocándose en satisfacer a los usuarios más importantes.
*   **Contar las historias de los usuarios (el flujo narrativo)**: La historia de un usuario se cuenta de **izquierda a derecha**, mostrando el flujo de actividades. Las **grandes actividades o el "backbone" (columna vertebral)** se ubican en la parte superior del mapa.
*   **Explorar detalles y opciones (la profundidad)**: Debajo de cada gran paso de usuario, se desglosan los **detalles más pequeños o las alternativas** (de arriba hacia abajo). Es clave mantener el enfoque en la **amplitud de la historia ("kilometer wide, centimeter deep") antes de profundizar en los detalles**.
*   **Beneficios del mapeo de historias**:
    *   Ayuda a **construir un entendimiento compartido** dentro del equipo y con las partes interesadas.
    *   Permite **identificar "agujeros" o aspectos no considerados** en el pensamiento inicial, entendiendo que "el alcance no se arrastra; el entendimiento crece".
    *   Facilita la visualización de una **"perspectiva general" (big picture) del producto completo**.
    *   Sirve como una **herramienta para organizar conversaciones**.
    *   Es una forma de **descomponer historias grandes en otras más pequeñas**.
*   **Caso de estudio "Artgility"**: The Learning Connexion, una escuela de arte, utilizó el mapeo de historias para comprender su propio proceso de gestión de estudiantes, lo que les permitió visualizar el proceso completo, entender su rol en él y **desarrollar un lenguaje común y un entendimiento compartido**. Esto les ayudó a identificar qué era **vital para la primera versión** del software.

En síntesis, el Capítulo 1 enfatiza que el mapeo de historias es una **forma colaborativa y visual de construir un entendimiento compartido** sobre un producto, permitiendo a los equipos ver la "perspectiva general" y desglosar ideas grandes en partes manejables, mientras se enfocan en **resolver problemas y "cambiar el mundo"** para los usuarios.

# Resumen: Capítulo 2, "Plan to Build Less"

El Capítulo 2, titulado "Plan to Build Less" (Planificar para construir menos), se centra en la realidad ineludible de que **"siempre hay más para construir de lo que se tiene tiempo o recursos"**. La solución que propone el capítulo para gestionar esta realidad es el **mapeo de historias** (story mapping), que permite a los colaboradores pensar en alternativas y lograr resultados positivos con los recursos disponibles.

Las ideas principales del Capítulo 2 son:

*   **La inevitabilidad de "demasiado para construir"**: En el desarrollo de software, siempre hay más cosas que construir de las que se tiene tiempo o recursos. El verdadero objetivo no es construir más rápido, sino **construir menos**. La clave es **minimizar la producción (output) y maximizar el resultado (outcome) y el impacto**.
*   **El mapeo ayuda a grandes grupos a construir entendimiento compartido**: El mapeo de historias es crucial para equipos grandes y diversos, como el caso de Globo.com. Permite visualizar todas las dependencias y la totalidad del trabajo necesario para un lanzamiento conjunto. Al organizar los *backlogs* individuales en un solo mapa, los equipos pueden ver cómo su trabajo encaja en el panorama general del producto.
*   **Anatomía de un mapa grande**: Un mapa de historias típico tiene una **"columna vertebral" (backbone) en la parte superior** que organiza el mapa en grandes actividades o pasos de usuario. Estos pasos cuentan una historia narrativa de izquierda a derecha sobre lo que los usuarios hacen en el sistema. Debajo de estos, se desglosan los detalles más pequeños.
*   **El mapeo revela "agujeros" en el entendimiento**: Al construir mapas de historias, los equipos a menudo descubren **vacíos o aspectos no considerados** en su planificación inicial. Esto no es "desvío del alcance" (scope creep), sino un **crecimiento del entendimiento**. Permite identificar problemas o necesidades que de otro modo habrían surgido más tarde.
*   **Cómo "cortar" un lanzamiento de Producto Mínimo Viable (MVP)**:
    *   La pregunta clave no es si se necesita construir todo, sino **cuándo**. Los equipos deben centrarse en los **resultados (outcomes) deseados**, es decir, lo que se espera que suceda fuera del sistema para los usuarios.
    *   Se utiliza cinta o líneas horizontales para **"cortar" (slice out) el mapa**, designando qué elementos se incluirán en el primer lanzamiento y cuáles se harán más tarde.
    *   Cada "corte" se enfoca en un **resultado específico** para los usuarios.
    *   Esto lleva a una **hoja de ruta de lanzamientos incrementales**, donde cada lanzamiento ofrece un beneficio real y medible, priorizando los beneficios del mundo real sobre una lista de características.
*   **Priorizar resultados, no características**: El secreto para priorizar el trabajo de desarrollo es **centrarse en resultados específicos**. Si no se conocen los resultados buscados, la priorización se vuelve casi imposible. El caso de Globo.com ilustra cómo la concentración en un resultado específico (las elecciones brasileñas) les permitió definir su primer lanzamiento, aunque significara dejar fuera a otros usuarios temporalmente.
*   **Definiendo el Producto Mínimo Viable (MVP)**:
    *   El MVP **no es "el producto más cutre que se pueda lanzar"**.
    *   La definición preferida es **"la versión más pequeña del producto que logra con éxito los resultados deseados"**. Esto requiere ser específico sobre a quién está dirigido y qué necesitan lograr.
    *   Para nuevas características o mejoras, se prefiere el término **"solución mínima viable"** (minimum viable solution).
    *   Finalmente, el capítulo introduce una tercera definición de MVP, popularizada por Eric Ries: **"el elemento más pequeño que se puede crear o hacer para probar o refutar una suposición"**. Esto transforma cada lanzamiento en un **experimento (MVPe)** cuyo objetivo principal es aprender y validar suposiciones.

En esencia, el Capítulo 2 enseña que el mapeo de historias es una **herramienta poderosa para planificar estratégicamente**, permitiendo a los equipos **visualizar el panorama completo, identificar lo esencial y priorizar en función de los resultados deseados**, en lugar de simplemente crear una lista interminable de características. Esto ayuda a **"construir menos"** pero con un impacto mucho mayor.
