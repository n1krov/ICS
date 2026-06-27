---
title: "Eventos de SCRUM"
author: "What a Scrummy Man..."
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
  - \usepackage{tabularx}
  - \usepackage{array}
  - \renewcommand{\arraystretch}{1.5}
  
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

# EVENTOS DE SCRUM Y ROLES QUE PARTICIPAN

## 1. **Sprint**

* **Descripción**: Es el contenedor de todos los demás eventos. Es un ciclo de tiempo fijo (timebox) de máximo 1 mes donde se crea un incremento del producto usable y potencialmente entregable.
* **Participan**:
  Todo el **Scrum Team**:

  * **Product Owner**
  * **Scrum Master**
  * **Developers**

---

## 2. **Sprint Planning**

* **Descripción**: Reunión que da inicio al Sprint. Se define el objetivo del Sprint (**Sprint Goal**), qué elementos del Product Backlog se van a trabajar y cómo se va a llevar a cabo el trabajo.
* **Participan**:
  Todo el **Scrum Team**
  (PO, Scrum Master, Developers)

---

## 3. **Daily Scrum**

* **Descripción**: Reunión diaria de 15 minutos donde los Developers inspeccionan el progreso hacia el Sprint Goal y ajustan el plan de trabajo si es necesario.
* **Participan**:
  **Developers**

  > El **Scrum Master** y el **Product Owner** pueden asistir, **pero no intervienen** a menos que estén colaborando como Developers.

---

### Aclaración sobre los participantes de la Daily Scrum.

*¿Por qué dice que el Scrum Master y el Product Owner pueden asistir pero no intervienen?*

Porque:

1. **La Daily Scrum es un evento exclusivo de los Developers.**

   * Es **de ellos para ellos**.
   * Es donde se autoorganizan, se alinean y deciden qué hacer para lograr el objetivo del Sprint.

2. **El Scrum Master puede asistir para garantizar que se respete el marco de Scrum** (por ejemplo, que no se vuelva una reunión de reporte al jefe).

   * Pero **no dirige** la reunión ni la utiliza para controlar al equipo.

3. **El Product Owner puede asistir para observar** o incluso responder preguntas **si los Developers lo requieren**, pero **no participa activamente**.

   * No debe usar la Daily para presionar o negociar.

---

### ¿Y cuándo podrían intervenir?

Solo **si están colaborando activamente como Developers** en ese Sprint (por ejemplo, si están ayudando a codificar, probar o diseñar). En ese caso, son parte del equipo de desarrollo y participan como uno más.

---

### En resumen

> En la Daily Scrum, **el foco está 100% en los Developers**. El Scrum Master y el Product Owner pueden estar presentes, pero **solo observan**, **no interfieren ni conducen la reunión**, a menos que **participen activamente como Developers**.

## 4. **Sprint Review**

* **Descripción**: Al final del Sprint, se presenta el incremento terminado a los stakeholders y se revisa el progreso hacia el Product Goal.
* **Participan**:
  Todo el **Scrum Team**
  **Stakeholders** (invitados por el PO)

---

### 5. **Sprint Retrospective**

* **Descripción**: Reunión para que el Scrum Team inspeccione cómo fue el Sprint en términos de personas, procesos y herramientas, y definan mejoras para el próximo Sprint.
* **Participan**:
  Todo el **Scrum Team**

---

## Resumen en tabla

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{4.5cm}|p{9.5cm}|}
\hline
\textbf{Evento} & \textbf{Participantes principales} \\
\hline
\textbf{Sprint} & Scrum Team (PO, Scrum Master, Developers) \\
\hline
\textbf{Sprint Planning} & Scrum Team \\
\hline
\textbf{Daily Scrum} & Developers (el Scrum Master y PO pueden asistir) \\
\hline
\textbf{Sprint Review} & Scrum Team + Stakeholders (si el PO los invita) \\
\hline
\textbf{Sprint Retrospective} & Scrum Team \\
\hline
\end{tabular}
\caption{Eventos de Scrum y sus participantes principales}
\end{table}

---
