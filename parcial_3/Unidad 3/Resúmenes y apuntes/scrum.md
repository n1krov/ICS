---
title: "Ingeniería y Calidad de Software"
author: "Billy y Mandy"
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

# Scrum

Según la Guía Scrum de noviembre de 2020, escrita por Ken Schwaber y Jeff Sutherland, **Scrum es un marco de trabajo ligero que ayuda a las personas, equipos y organizaciones a generar valor a través de soluciones adaptables para problemas complejos**.

Aquí te presento una explicación detallada de Scrum, basándome en la Guía Scrum 2020:

## **Propósito de la Guía Scrum:**

* La Guía Scrum fue desarrollada a principios de la década de 1990 y su primera versión fue escrita en 2010 para ayudar a las personas de todo el mundo a entender Scrum.
* Ha evolucionado a través de pequeñas actualizaciones funcionales.
* Contiene la definición de Scrum, y cada elemento del marco tiene un propósito específico que es esencial para el valor global y los resultados obtenidos.
* Cambiar el diseño, las ideas básicas o las reglas de Scrum, o dejar fuera elementos, puede cubrir problemas y limitar sus beneficios, incluso haciéndolo inútil.
* Aunque Scrum tiene sus raíces en el desarrollo de productos de software, se ha adoptado en muchos dominios con trabajo esencialmente complejo. La palabra "desarrolladores" se usa para simplificar, incluyendo a todos los especialistas que obtienen valor de Scrum.

## **Naturaleza y Filosofía de Scrum:**

* **Scrum es simple** y se debe probar tal cual para determinar si su filosofía, teoría y estructura ayudan a alcanzar metas y crear valor.
* Es un marco **deliberadamente incompleto**, que solo define las partes necesarias para implementar su teoría. Se basa en la inteligencia colectiva de las personas que lo utilizan y sus reglas guían las relaciones e interacciones en lugar de proporcionar instrucciones detalladas.
* Dentro del marco de Scrum, se pueden emplear diversos procesos, técnicas y métodos. Scrum envuelve prácticas existentes o las hace innecesarias, y hace visible la eficacia relativa de la gestión actual, el entorno y las técnicas de trabajo, permitiendo mejoras.
* **Se basa en el empirismo y el pensamiento Lean**.
	* **Empirismo**: Afirma que el conocimiento proviene de la experiencia y la toma de decisiones basadas en lo que se observa.
	* **Pensamiento Lean**: Reduce los desperdicios y se centra en lo esencial.
* Emplea un **enfoque iterativo e incremental** para optimizar la previsibilidad y controlar el riesgo.

## **Los Pilares de Scrum:**

Los eventos de Scrum funcionan porque implementan los tres pilares empíricos:

### **Transparencia**

El proceso y el trabajo emergentes deben ser visibles para quienes realizan el trabajo y para quienes lo reciben. Decisiones importantes se basan en el estado percibido de los tres artefactos formales de Scrum. La falta de transparencia puede llevar a decisiones que disminuyen el valor y aumentan el riesgo. La transparencia permite la inspección.

### **Inspección**

Los artefactos de Scrum y el progreso hacia los objetivos acordados deben ser inspeccionados con frecuencia y diligentemente para detectar variaciones o problemas indeseables. Scrum proporciona cadencia a través de sus cinco eventos para ayudar en la inspección. La inspección permite la adaptación.

### **Adaptación**

Si algún aspecto de un proceso se desvía de los límites aceptables o si el producto resultante es inaceptable, el proceso o los materiales deben ajustarse lo antes posible para minimizar desviaciones adicionales. El equipo Scrum se adapta en el momento en que aprende algo nuevo por medio de la inspección.

## **Valores de Scrum:**

El éxito de Scrum depende de que las personas vivan cinco valores:

### **Compromiso**

El equipo se compromete a lograr sus objetivos y apoyarse mutuamente.

### **Enfoque**

Su enfoque principal es el trabajo del Sprint para hacer el mejor progreso posible hacia los objetivos.

### **Apertura**

El equipo y sus partes interesadas están abiertos sobre el trabajo y los desafíos.

### **Respeto**

Los miembros del equipo se respetan mutuamente como personas capaces e independientes, y son respetados como tales por quienes trabajan con ellos.

### **Coraje**

Los miembros del equipo tienen el coraje de hacer lo correcto y de trabajar en problemas complejos.

Estos valores dan dirección al equipo Scrum y refuerzan los pilares empíricos, construyendo confianza.

## **El Equipo Scrum (Scrum Team):**

* Es la **unidad fundamental de Scrum**, un pequeño equipo de personas.
* Consta de un **Scrum Master, un Propietario de Producto (Product Owner) y Desarrolladores**.
* **No hay sub-equipos ni jerarquías** dentro de un equipo Scrum; es una unidad cohesionada de profesionales enfocada en un objetivo a la vez (el Objetivo del Producto).
* Son **multifuncionales**, lo que significa que los miembros tienen todas las habilidades necesarias para crear valor en cada Sprint.
* Son **autogestionados**, lo que significa que internamente deciden quién hace qué, cuándo y cómo.
* Suelen ser de **10 o menos personas** para permanecer ágiles. Si los equipos se vuelven demasiado grandes, se considera reorganizarse en varios equipos Scrum cohesionados, cada uno centrado en el mismo producto.
* Son responsables de todas las actividades relacionadas con el producto y están empoderados por la organización para gestionar su propio trabajo.

### **Responsabilidades Específicas del Equipo Scrum:**

1.  **Desarrolladores**:

	* Son las personas del equipo Scrum que se comprometen a **crear cualquier aspecto de un Incremento útil** en cada Sprint.
	* Son responsables de: crear el plan del Sprint (Sprint Backlog), inculcar la calidad adhiriéndose a una Definición de Hecho, adaptar su plan cada día hacia el Objetivo Sprint, y responsabilizarse mutuamente como profesionales.

2.  **Propietario del Producto (Product Owner)**:

	* Es **responsable de maximizar el valor del producto** resultante del trabajo del equipo Scrum.
	* También es responsable de la **gestión eficaz de la Pila del Producto (Product Backlog)**, incluyendo: desarrollar y comunicar el Objetivo del Producto, crear y comunicar elementos claros, ordenar los elementos y asegurar que la Pila del Producto sea transparente, visible y comprendida.
	* Puede delegar el trabajo, pero sigue siendo el responsable.
	* Es una persona, no un comité.

3.  **Scrum Master**:

	* Es **responsable de establecer Scrum** tal como se define en la Guía. Lo logra ayudando a todos a comprender la teoría y la práctica de Scrum, tanto dentro del Equipo como en toda la organización.
	* Es responsable de la **efectividad del Scrum Team**, permitiendo que mejore sus prácticas dentro del marco de Scrum.
	* Sirve al equipo de Scrum (capacitando en autogestión, ayudando a enfocarse, eliminando impedimentos, asegurando que los eventos sean productivos y respeten su tiempo).
	* Sirve al Propietario del Producto (ayudando en la definición de objetivos, gestión del Product Backlog, planificación empírica y colaboración con stakeholders).
	* Sirve a la organización (liderando la adopción de Scrum, planificando la implementación y eliminando barreras).

## **Eventos de Scrum:**

* El **Sprint es un contenedor para todos los eventos**. Cada evento es una oportunidad formal para inspeccionar y adaptar los artefactos de Scrum, diseñados para permitir la transparencia.
* Los eventos se realizan óptimamente al mismo tiempo y lugar para reducir la complejidad.

### 1.  **El Sprint**:

* Son el **latido del corazón de Scrum**, donde las ideas se convierten en valor.
* Son de **longitud fija, de un mes o menos**, para crear consistencia. Un nuevo Sprint comienza inmediatamente después del anterior.
* Todo el trabajo necesario para alcanzar el Objetivo del Producto ocurre dentro del Sprint.
* Durante el Sprint: no se hacen cambios que pongan en peligro el Objetivo Sprint; la calidad no disminuye; el Product Backlog se refina; el alcance puede clarificarse y renegociarse.
* Permiten la previsibilidad y limitan el riesgo. Un Sprint puede cancelarse si el Objetivo del Sprint se vuelve obsoleto, y solo el Product Owner tiene la autoridad para cancelarlo.

### 2.  **Planificación de Sprint (Sprint Planning)**:

* Inicia el Sprint y establece el trabajo a realizar. Es un **trabajo colaborativo de todo el equipo Scrum**.
* Aborda tres temas:
	* **Tema Uno: ¿Por qué este Sprint es valioso?** El Product Owner propone cómo el producto podría aumentar su valor, y el equipo Scrum define el Objetivo de Sprint.
	* **Tema Dos: ¿Qué se puede hacer este Sprint?** Los Desarrolladores seleccionan elementos del Product Backlog con el Product Owner.
	* **Tema Tres: ¿Cómo se realizará el trabajo elegido?** Los Desarrolladores planifican el trabajo, descomponiendo los elementos del Product Backlog en tareas más pequeñas (un día o menos).
* La duración máxima es de **ocho horas para un Sprint de un mes**.

### 3.  **Scrum Diario (Daily Scrum)**:

* Su propósito es **inspeccionar el progreso hacia el Objetivo Sprint y adaptar el Sprint Backlog**.
* Es un evento de **15 minutos (máximo) para los Desarrolladores**, que se celebra a la misma hora y lugar cada día laboral del Sprint.
* Se centra en el progreso hacia el Objetivo de Sprint y produce un plan accionable para el día siguiente.
* Mejora la comunicación, identifica impedimentos y promueve la toma rápida de decisiones.

### 4.  **Revisión del Sprint (Sprint Review)**:

* Su propósito es **inspeccionar el resultado del Sprint y determinar futuras adaptaciones**.
* El equipo Scrum presenta los resultados a las partes interesadas clave y discuten el progreso hacia el Objetivo de Producto.
* Es una **sesión de trabajo colaborativa** donde se revisa lo logrado y los cambios en el entorno, y se decide qué hacer a continuación. El Product Backlog puede ajustarse.
* Es el penúltimo evento del Sprint, con una duración máxima de **cuatro horas para un Sprint de un mes**.

### 5.  **La Retrospectiva del Sprint (Sprint Retrospective)**:

* Su propósito es **planificar formas de aumentar la calidad y la eficacia**.
* El equipo Scrum inspecciona cómo fue el Sprint anterior (individuos, interacciones, procesos, herramientas y Definición de Hecho), identificando lo que fue bien, los problemas y cómo se resolvieron.
* Identifican los cambios más útiles para mejorar su eficacia, que pueden agregarse al Sprint Backlog para el próximo Sprint.
* Concluye el Sprint, con una duración máxima de **tres horas para un Sprint de un mes**.

## **Artefactos de Scrum:**

Los artefactos representan trabajo o valor y están diseñados para maximizar la transparencia de la información clave. Cada artefacto contiene un "compromiso" para asegurar que proporciona información que mejora la transparencia y el enfoque.

### 1.  **Pila del Producto (Product Backlog)**:

* Es una **lista emergente y ordenada de lo que se necesita para mejorar el producto**. Es la única fuente de trabajo emprendida por el equipo Scrum.
* Los elementos listos para ser seleccionados en la Planificación de Sprint generalmente adquieren este grado de transparencia después de actividades de refinamiento. El refinamiento es una actividad continua para descomponer y definir elementos, añadiendo detalles.
* **Compromiso: Objetivo del Producto (Product Goal)**: Describe un estado futuro del producto que sirve como objetivo a largo plazo para el equipo Scrum. El resto del Product Backlog surge para definir "qué" cumplirá este objetivo.

### 2.  **La Pila del Sprint (Sprint Backlog)**:

* Se compone del **Objetivo Sprint (por qué), el conjunto de elementos del Product Backlog seleccionados para el Sprint (qué), y un plan accionable para entregar el Incremento (cómo)**.
* Es un plan por y para los Desarrolladores, visible y en tiempo real del trabajo que planean realizar. Se actualiza a lo largo del Sprint a medida que se aprende más.
* **Compromiso: Sprint Goal**: Es el **único objetivo para el Sprint**. Proporciona flexibilidad en el trabajo exacto necesario para lograrlo y crea coherencia y enfoque para que el equipo trabaje junto.

### 3.  **Incremento (Increment)**:

* Es un **paso concreto hacia el Objetivo del Producto**. Cada Incremento es aditivo a todos los anteriores y está verificado, asegurando que todo funcione junto.
* Para proporcionar valor, el Incremento **debe ser utilizable**.
* Se pueden crear varios Incrementos dentro de un Sprint, y la suma de ellos se presenta en la Revisión de Sprint. Un Incremento puede ser entregado a las partes interesadas antes del final del Sprint.
* El trabajo no se considera parte de un Incremento a menos que cumpla con la Definición de Hecho.
* **Compromiso: Definición de Hecho (Definition of Done)**: Es una **descripción formal del estado del Incremento cuando cumple con las medidas de calidad** requeridas para el producto. Crea transparencia al proporcionar una comprensión compartida de qué trabajo se completó. Si un elemento no cumple con esta definición, no puede ser liberado ni presentado en la Revisión de Sprint; vuelve al Product Backlog.

## **Nota Final de la Guía Scrum 2020:**

* Scrum es gratuito y el **marco es inmutable**. Implementar solo algunas partes no es Scrum; Scrum solo existe en su totalidad y funciona bien como un contenedor para otras técnicas, metodologías y prácticas.

**Cambios relevantes en la versión 2020 de la Guía Scrum:**

* **Menos prescriptiva**: Busca ser un marco mínimamente válido y suficiente, eliminando o suavizando el lenguaje prescriptivo (ej., preguntas eliminadas del Daily Scrum, lenguaje suavizado sobre atributos del Product Backlog).
* **Un equipo, centrado en un producto**: Se elimina el concepto de "equipo de desarrollo" separado, consolidando a todos en un único Equipo Scrum con tres categorías de responsabilidades: Product Owner, Scrum Master y Desarrolladores.
* **Introducción del Objetivo del Producto**: Permite que el Equipo Scrum se enfoque en un objetivo más grande y con más valor, al cual cada Sprint debe acercar el producto.
* **Compromisos para los artefactos**: Se da mayor claridad a la identidad del Objetivo de Sprint, la Definición de Hecho y el Objetivo del Producto, asociándolos como "compromisos" a cada uno de los tres artefactos, reforzando el empirismo y los valores.
* **Autogestión en lugar de auto-organización**: Se enfatiza que el Equipo Scrum se autogestiona, eligiendo quién, cómo y dónde trabajar.
* **Tres temas en la planificación del Sprint**: Se añade y enfatiza un tercer tema ("Por qué" o Objetivo del Sprint), además de los existentes "Qué" y "Cómo".
* **Simplificación general del lenguaje**: Se eliminan frases redundantes, complejas y las influencias restantes del mundo de las TIC (ej., pruebas, sistemas, diseños, requisitos), resultando en una guía más corta.
