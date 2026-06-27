---
title: "Normas de calidad"
author: "GuISO"
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

# Clasificación de normas y modelos: **Producto vs. Proceso**

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabularx}{\textwidth}{|p{4.5cm}|c|c|X|}
\hline
\textbf{Norma / Modelo} & \textbf{¿Producto?} & \textbf{¿Proceso?} & \textbf{Comentario breve} \\
\hline
\textbf{ISO/IEC 25000} & Sí & No & Marco para evaluar la calidad del producto de software \\
\textbf{ISO/IEC 25010} & Sí & No & Define el modelo de calidad del producto y en uso \\
\textbf{CISQ} & Sí & No & Modelo americano centrado en calidad del producto \\
\textbf{ISO/IEC 12207} & No & Sí & Modelo de referencia de procesos (define qué procesos seguir) \\
\textbf{ISO/IEC 15504 (SPICE)} & No & Sí & Modelo de evaluación de procesos (antecesor de ISO 33000) \\
\textbf{ISO/IEC 33000} & No & Sí & Nueva versión de SPICE. Modelo de evaluación de procesos \\
\textbf{ISO/IEC 29110} & No & Sí & Modelo de procesos para pequeñas organizaciones \\
\textbf{CMMI} & No & Sí & Modelo de madurez para procesos de desarrollo \\
\textbf{SonarQ / CAST / Kiuwan} & Sí & No & Herramientas para medir calidad de código/producto \\
\textbf{Modelo propio + herramientas + proceso de evaluación} & Sí & Sí & Cuando se combinan ambos enfoques en una organización \\
\hline
\end{tabularx}
\end{table}

---

# ¿Existe alguna norma que abarque *ambas* dimensiones?

**No hay una norma individual que cubra completamente *producto* y *proceso* a la vez**, pero **sí se pueden integrar modelos y herramientas para abordarlas juntas**. Por ejemplo:

* Una organización puede usar **ISO 12207** + **ISO 33000** para trabajar en procesos,
  y combinarlo con **ISO 25010/25000** + herramientas como SonarQ para evaluar productos.

Entonces, **la integración de ambos enfoques** (producto y proceso) es lo que permite:

* Asegurar calidad en el desarrollo **durante el proceso**
* Evaluar y certificar la calidad del **producto final**

---

# Conclusión clave (según el video)

> **La calidad del proceso y del producto están profundamente relacionadas**, aunque se gestionan con normas distintas. Una buena gestión de procesos (como pruebas, análisis, requisitos) **incrementa la probabilidad de obtener un producto final de calidad**.
