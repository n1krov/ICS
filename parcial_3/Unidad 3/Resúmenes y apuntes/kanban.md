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

# Kanban 

# Valores

Los valores de Kanban son 9: **Transparency**, **Balance**, **Collaboration**, **Consumer** **Focus**, **Flow**, **Leadership**, **Understanding**, **Agreement**, **Respect**.

> *Memory Maker: *T*omás *B*ebió *C*erveza *C*on *F*ernet, *L*uego *U*só *A*lmohadas *R*aras.*

---

### 1. **Transparencia**

> La creencia de que compartir información de forma abierta mejora el flujo de valor del negocio.

* Implica utilizar un lenguaje claro y accesible.
* Permite que todos los involucrados comprendan el estado del trabajo, los bloqueos y las prioridades.
* Refuerza la confianza y facilita la toma de decisiones informadas.

---

### 2. **Balance**

> Comprender que se deben equilibrar diferentes aspectos, perspectivas y capacidades para ser efectivos.

* Ejemplo: mantener un equilibrio entre la **demanda** (trabajo solicitado) y la **capacidad** (recursos disponibles).
* El desequilibrio sostenido puede llevar a cuellos de botella, burnout o pérdida de valor.

---

### 3. **Colaboración**

> Trabajar juntos es el corazón de Kanban.

* No se trata solo de trabajar en equipo, sino de mejorar **cómo trabajamos juntos**.
* Kanban promueve prácticas que fomentan la interacción y el aprendizaje colectivo.

---

### 4. **Enfoque en el Cliente**

> Tener claro el objetivo del sistema: **entregar valor al cliente**.

* El flujo de trabajo en Kanban siempre apunta a satisfacer una necesidad externa o interna.
* Mantener al cliente en el centro guía la priorización y las mejoras del proceso.

---

### 5. **Flujo**

> Ver el trabajo como un flujo continuo (o episódico) de valor.

* El objetivo es **visualizar y optimizar ese flujo** para que sea más eficiente y predecible.
* Observar el flujo ayuda a identificar bloqueos y oportunidades de mejora.

---

### 6. **Liderazgo**

> Inspirar a otros mediante el ejemplo, la palabra y la reflexión.

* Kanban no depende solo del liderazgo jerárquico.
* Se necesita **liderazgo en todos los niveles** (líderes técnicos, facilitadores, miembros del equipo) para promover la mejora continua.

---

### 7. **Comprensión**

> Autoconocimiento (personal y organizacional) como base del cambio.

* Para mejorar, primero hay que **entender cómo funciona el sistema actual**.
* Kanban se basa en observar antes de actuar: primero comprender, luego evolucionar.

---

### 8. **Acuerdo**

> Compromiso colectivo para avanzar hacia objetivos comunes.

* Implica respetar diferencias y buscar **alineamiento dinámico**, no necesariamente consenso total.
* El equipo se compromete a mejorar, incluso cuando no todos piensan igual.

---

### 9. **Respeto**

> Valorar y considerar a las personas.

* Es el **valor fundamental** en el que se apoyan todos los demás.
* Implica reconocer el trabajo de los demás, sus roles, sus límites y su contexto.

---

### Conclusión

Estos valores no son opcionales ni decorativos:

> **Son esenciales para aplicar Kanban con fidelidad.**

* Ayudan a crear un entorno de trabajo sostenible, adaptativo y centrado en el cliente.
* Sin estos valores, el uso de tableros y límites WIP se vuelve mecánico y pierde su verdadero propósito.

---

# Principios

Los **6 principios fundamentales de Kanban** se dividen en dos grupos: **Principios de Gestión del Cambio** y **Principios de Entrega de Servicios**.

## **Principios de Gestión del Cambio** (Change Management Principles)

Estos principios guían **cómo introducir Kanban** de manera evolutiva y respetuosa:

### 1. **Comenzar con lo que haces ahora**

(*Start with what you do now*)

* Se parte de los procesos **reales existentes**, tal como se practican hoy.
* Se **respetan los roles, responsabilidades y estructuras actuales**.
* Esto minimiza la resistencia al cambio y permite evolucionar desde la realidad, no desde teorías.

---

### 2. **Aceptar buscar mejoras a través del cambio evolutivo**

(*Agree to pursue improvement through evolutionary change*)

* El cambio debe ser **gradual y constante**, no disruptivo ni impuesto.
* Se basa en **experimentos controlados**, aprendizaje continuo y ajustes incrementales.

---

### 3. **Fomentar actos de liderazgo en todos los niveles**

(*Encourage acts of leadership at every level*)

* El liderazgo no es exclusivo de los gerentes.
* Se promueve que **todas las personas contribuyan a la mejora**, ya sea un desarrollador, analista, tester o líder técnico.

---

## **Principios de Entrega de Servicios** (Service Delivery Principles)

Estos principios se enfocan en **cómo entregar valor al cliente de forma eficiente**:

### 4. **Entender y enfocarse en las necesidades y expectativas del cliente**

(*Understand and focus on your customers’ needs and expectations*)

* Todo servicio debe orientarse a **satisfacer lo que el cliente espera**.
* Se deben visualizar y gestionar los elementos de trabajo que **realmente entregan valor**.

---

### 5. **Gestionar el trabajo, permitir que las personas se autoorganicen**

(*Manage the work; let people self-organize around it*)

* Se gestiona el **flujo de trabajo**, no a las personas.
* Se confía en que los equipos se organizarán mejor si comprenden el contexto y los objetivos.

---

### 6. **Evolucionar las políticas para mejorar resultados de negocio y cliente**

(*Evolve policies to improve customer and business outcomes*)

* Las **políticas (reglas, límites, acuerdos)** deben ser **explícitas**, pero también **flexibles**.
* Deben evolucionar según el aprendizaje, los resultados y el entorno cambiante.

---

### Resumen visual:

+--------------------------+------------------------------------------------------------------+
| Tipo de Principio        | Principios                                                       |
+==========================+==================================================================+
| **Gestión del Cambio**   | 1. Empezar con lo que hacés ahora                                |
|                          | 2. Mejorar de forma evolutiva                                    |
|                          | 3. Liderazgo en todos los niveles                                |
+--------------------------+------------------------------------------------------------------+
|                          |                                                                  |
+--------------------------+------------------------------------------------------------------+
| **Entrega de Servicios** | 4. Enfocarse en el cliente                                       |
|                          | 5. Gestionar el trabajo, no personas                             |
|                          | 6. Evolucionar políticas para mejorar                            |
+--------------------------+------------------------------------------------------------------+

---

## Prácticas Generales

En el libro ***Essential Kanban Condensed***, las **"General Practices of Kanban"** (Prácticas Generales de Kanban) son seis actividades fundamentales que permiten **gestionar y mejorar un sistema de flujo de trabajo**. Estas prácticas son válidas para cualquier tipo de servicio, pero son especialmente útiles en entornos de trabajo del conocimiento, como el desarrollo ágil de software.

---

### 1. **Visualizar**

> *“Visualize”*

* Mostrar el trabajo y el proceso por el que pasa.
* Se hace típicamente con un **tablero Kanban**, que muestra columnas (estados) y tarjetas (items de trabajo).
* También se visualizan **políticas y bloqueos** (por ejemplo, tareas detenidas por dependencias).

*¿Por qué?*
Porque **lo que no se ve, no se puede gestionar ni mejorar**.

---

### 2. **Limitar el trabajo en progreso (WIP)**

> *“Limit Work in Progress”*

* Se establece un **límite máximo** de tareas que pueden estar activas en cada columna.
* Esto transforma el sistema en un **sistema pull**, donde el trabajo entra solo si hay capacidad.

*¿Por qué?*
Reducir el WIP mejora el **tiempo de entrega**, la calidad y **evita sobrecargar al equipo**.

---

### 3. **Gestionar el flujo**

> *“Manage Flow”*

* Observar cómo fluye el trabajo a través del sistema, con foco en:

  * *Lead time* (tiempo de entrega),
  * bloqueos,
  * cuellos de botella.

*¿Por qué?*
Para **maximizar la entrega de valor** y responder rápido ante problemas.

---

### 4. **Hacer explícitas las políticas**

> *“Make Policies Explicit”*

* Las reglas de cómo se trabaja deben estar **claras, visibles y compartidas**.
* Ejemplos: definición de “hecho”, reglas de prioridad, criterios para mover tarjetas.

*¿Por qué?*
Porque las **reglas claras reducen ambigüedades** y permiten evaluar/mejorar el proceso.

---

### 5. **Implementar ciclos de retroalimentación**

> *“Implement Feedback Loops”*

* Incluir **revisiones periódicas**:

  * Daily Kanban,
  * Replenishment meeting,
  * Service Delivery Review, etc.

*¿Por qué?*
Para **coordinar al equipo**, alinear con el negocio y guiar la mejora continua.

---

### 6. **Mejorar colaborativamente, evolucionar experimentalmente**

> *“Improve Collaboratively, Evolve Experimentally”*

* El equipo analiza el sistema, genera hipótesis y hace **experimentos controlados** para mejorar.
* Se basa en modelos, datos y la experiencia del equipo.

*¿Por qué?*
Porque **la mejora sostenible se logra iterando, aprendiendo y adaptando**.

---

### Resumen visual:

| Nº | Práctica Kanban                                   | Propósito principal                                   |
| -- | ------------------------------------------------- | ----------------------------------------------------- |
| 1  | Visualizar                                        | Hacer visible el trabajo y el proceso                 |
|                                                                                                                |
| 2  | Limitar WIP                                       | Evitar sobrecarga, reducir tiempos, crear foco        |
|                                                                                                                |
| 3  | Gestionar el flujo                                | Entregar valor de forma fluida y predecible           |
|                                                                                                                |
| 4  | Hacer explícitas las políticas                    | Aumentar claridad, coherencia y transparencia         |
|                                                                                                                |
| 5  | Implementar ciclos de retroalimentación           | Coordinar, alinear y mejorar                          |
|                                                                                                                |
| 6  | Mejorar colaborativamente y evolucionar con datos | Impulsar el cambio continuo basado en experimentación |

---
