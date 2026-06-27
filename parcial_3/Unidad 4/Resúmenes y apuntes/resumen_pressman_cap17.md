---
title: "Ingeniería y Calidad de Software"
author: "Jake and Drosh"
date: "24-06-2025"
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

# Pressman: Estrategias de prueba de software

Los aspectos más fundamentales del Capítulo 17 sobre la estrategia de pruebas de software se pueden sintetizar en los siguientes puntos clave:

---

### 1. **Propósito de la prueba en el proceso de calidad**

La prueba de software se entiende como un conjunto **sistemático y planificado de actividades** que permiten evaluar la calidad del software. No se trata solo de encontrar errores, sino también de **verificar que el producto funcione correctamente** (verificación) y que **cumpla con lo que el cliente espera** (validación).

---

### 2. **Verificación y validación (V\&V)**

* **Verificación**: ¿Construimos bien el producto? Se enfoca en asegurar que el software implemente correctamente cada función.
* **Validación**: ¿Construimos el producto correcto? Se centra en comprobar que se satisfacen los requerimientos del usuario.

---

### 3. **Enfoque progresivo de la estrategia**

La estrategia de prueba se aplica en niveles:

* Comienza con **pruebas unitarias** (componentes individuales),
* Continúa con **pruebas de integración** (cómo se combinan esos componentes),
* Luego con **pruebas de validación** (comparación con requisitos),
* Y culmina en las **pruebas del sistema** (verificación completa del software).

---

### 4. **Fases clave de la estrategia de prueba**

#### a. **Prueba de unidad**

* Prueba del módulo más pequeño posible.
* Se verifica la lógica interna, manejo de errores y estructuras de datos.
* Se usan *stubs* y *drivers* para simular dependencias que aún no existen.

#### b. **Prueba de integración**

* Se integran módulos gradualmente, en vez de usar el enfoque “big bang”.
* Se usan controladores temporales para simular módulos aún no integrados.

#### c. **Prueba de validación**

* Evalúa si el sistema completo cumple con los requisitos funcionales y no funcionales.
* Incluye pruebas **alfa** (cliente en el entorno del desarrollador) y **beta** (cliente en su entorno real).

#### d. **Pruebas del sistema**

* Prueban el sistema en conjunto. Se evalúan:

  * Recuperación ante fallos,
  * Seguridad,
  * Resistencia ante sobrecarga,
  * Desempeño,
  * Instalación y configuración.

---

### 5. **La depuración como parte del proceso**

* Implica **detectar, localizar y corregir errores**.
* Requiere disciplina, ya que corregir un error puede introducir otros.
* Se utilizan estrategias como:

  * Fuerza bruta (poco eficaz),
  * Análisis hacia atrás desde el síntoma,
  * Eliminación sistemática de causas posibles.

---

### 6. **Importancia de una estrategia bien definida**

* Debe basarse en **requisitos cuantificables** desde las etapas tempranas del proyecto.
* Permite planificar, evaluar y mejorar la calidad del producto, no solo encontrar fallos.

---

En síntesis, el capítulo plantea que la prueba de software es un **proceso estructurado y fundamental para la calidad**, que debe abordarse desde varios niveles con distintas técnicas, y que incluye tanto el diseño de las pruebas como la gestión de errores mediante la depuración.
