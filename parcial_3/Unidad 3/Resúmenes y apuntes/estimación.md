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

## **Métodos paramétricos**

### ¿Qué son?

Son métodos que usan **datos cuantitativos históricos** y fórmulas para estimar esfuerzo, duración o costo. Se basan en **parámetros medibles**, como cantidad de historias, líneas de código, puntos de función, etc.

### ¿Cómo se aplican en ágil?

Aunque más comunes en gestión tradicional, se pueden usar en ágil si el equipo tiene **datos históricos de velocidad (velocity)** o métricas similares.

### **Ejemplo en contexto ágil:**

> Supongamos que tu equipo tiene una **velocidad promedio de 20 puntos por sprint**, y el backlog contiene 100 puntos estimados.
> **Cálculo paramétrico:**
>  100 puntos / 20 puntos por sprint = **5 sprints necesarios**

También podrías usar modelos como *COCOMO* (más tradicional) si estimás con líneas de código, aunque eso es poco frecuente en equipos ágiles puros.

---

##  **Métodos heurísticos**

###  ¿Qué son?

Se basan en **experiencia, juicio experto y reglas prácticas**, más que en fórmulas. Son rápidos y adaptables, aunque menos precisos.

###  ¿Cómo se aplican en ágil?

Muy comunes en metodologías ágiles. Se usan en:

* Estimación con **Planning Poker**
* Estimaciones con **t-shirt sizes** (S, M, L, XL)
* Evaluaciones rápidas basadas en experiencia pasada

###  **Ejemplo en contexto ágil:**

> El equipo revisa una historia y, basándose en su complejidad, la estima como **8 puntos**, porque es similar a otra que les llevó 2 días.

O bien:

> Usan talles:

* *Subir una imagen de perfil*: **S**
* *Implementar el sistema de pago completo*: **XL**

Estas estimaciones no son numéricas directamente, pero ayudan a **comparar esfuerzo relativo** y priorizar.

---

##  Comparación rápida:

| Característica         | Método Paramétrico              | Método Heurístico                      |
| ---------------------- | ------------------------------- | -------------------------------------- |
| Basado en datos reales |  Sí                            |  No necesariamente                    |
| Usa fórmulas           |  Sí                            |  No                                   |
| Rápido de aplicar      |  Puede no serlo               |  Sí                                   |
| Flexible               |  Menos                         |  Muy flexible                         |
| Común en ágil          |  Solo si hay métricas previas |  Sí, especialmente con Planning Poker |

---

###  Conclusión:

* Usá **paramétricos** si tenés **datos históricos confiables** (como velocidad o métricas similares).
* Usá **heurísticos** para estimaciones rápidas, comparativas y colaborativas durante **refinamientos o plannings**.

# Otros conceptos importantes

## Estimación y planificación ágil: conceptos fundamentales

### Puntos de historia

Los **puntos de historia** son una unidad de medida **subjetiva** utilizada para estimar el **esfuerzo relativo**, la **complejidad** o el **tamaño** de una historia de usuario. No representan horas ni días, sino que permiten al equipo comparar historias entre sí en términos de:

* Cantidad de trabajo
* Dificultad técnica
* Riesgos o incertidumbre

Este tipo de estimación ayuda a abstraerse del tiempo real y a centrarse en la naturaleza del trabajo.

---

### Escalas de estimación

En agilidad se utilizan escalas diseñadas para **resaltar las diferencias de tamaño** entre historias. Dos escalas comunes son:

* **Serie de Fibonacci modificada**: 1, 2, 3, 5, 8, 13, 21... (se omiten los más altos si son poco prácticos).
* **Escala personalizada o por talles**: S, M, L, XL, etc.

Ambas tienen el objetivo de evitar falsas sensaciones de precisión y **obligar al equipo a tomar decisiones conscientes sobre la complejidad** de cada historia.

---

### Valor de negocio

El **valor de negocio** es el **impacto positivo que una historia genera en el producto, usuario o cliente**. Aunque los puntos de historia estiman esfuerzo, el valor de negocio se utiliza para priorizar:

* ¿Qué historias aportan más valor con menos esfuerzo?
* ¿Qué funcionalidades son esenciales para el usuario o el mercado?

A veces se visualiza en una matriz valor/esfuerzo para tomar decisiones de priorización.

---

### Velocidad

La **velocidad** (velocity) es una medida empírica que representa **cuántos puntos de historia completa un equipo en un sprint**. Es única para cada equipo y depende de:

* Experiencia del equipo
* Herramientas disponibles
* Madurez del proceso
* Contexto del proyecto

La velocidad se calcula luego de varios sprints y se utiliza para **proyectar entregas futuras**.

Ejemplo:
Si el equipo entrega en promedio 25 puntos por sprint, y el backlog tiene 100 puntos, se estima que se necesitarán 4 sprints para completarlo.

---

### ¿Qué se necesita para poder estimar?

Para realizar una estimación útil en metodologías ágiles, es fundamental conocer:

* **Qué se va a hacer**: tener historias de usuario bien definidas.
* **El tamaño relativo de cada historia**: a través de puntos de historia o talles.
* **La velocidad del equipo**: determinada empíricamente tras varios sprints.

Con estas variables, es posible **planificar iteraciones**, establecer **releases progresivos** y **alinear expectativas** con stakeholders.
