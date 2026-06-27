---
title: "Ingeniería y Calidad de Software"
author: "Juani"
date: "08-05-2025"
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

## Diferencias entre **Definition of Done (DoD)** y **Criterios de Aceptación**

| Concepto            | Definition of Done (DoD)                                                   | Criterios de Aceptación                                                   |
|---------------------|------------------------------------------------------------------------------|------------------------------------------------------------------------------|
| Qué es              | Acuerdo común sobre cuándo una historia está completamente terminada.       | Condiciones específicas que una historia debe cumplir para ser aceptada.    |
| 	|
| Aplicación          | Se aplica a todas las historias del equipo.                                 | Específicos para cada historia de usuario.                                 |
| 	|
| Alcance             | Cubre aspectos generales como codificación, pruebas, documentación, etc.    | Cubre el comportamiento funcional esperado de la historia.                 |
| 	|
| Quién lo define     | El equipo de desarrollo (incluyendo QA, PO y SM).                           | Generalmente el Product Owner junto con el equipo.                         |
| 	|
| Propósito           | Garantizar calidad y coherencia en todas las entregas.                      | Asegurar que la historia cumple con lo que se espera funcionalmente.       |
| 	|
| Ejemplo             | La historia tiene tests, fue revisada y está desplegada en staging.         | Al hacer clic en "Guardar", se almacenan los datos y se muestra confirmación. |

---

## Una metáfora útil:

* El **DoD** es como una **checklist de fábrica** que asegura que cualquier producto que sale cumple con estándares mínimos de calidad.
* Los **criterios de aceptación** son como las **especificaciones del modelo particular** de ese producto.

---

## ¿Cómo se complementan?

1. **Los criterios de aceptación** aseguran que se está construyendo **lo correcto**.
2. **El DoD** asegura que se está construyendo **correctamente**.

Ambos se deben cumplir para que una historia se considere verdaderamente "terminada".

---
