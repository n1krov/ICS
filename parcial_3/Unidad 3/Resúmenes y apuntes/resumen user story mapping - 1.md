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

## **Capítulo 1: The Big Picture**

### Autor: Jeff Patton

---

### **Idea central:**

Muchas veces los equipos construyen software que técnicamente funciona, pero **no entrega valor real al usuario o al negocio**. Esto ocurre porque se pierde la **visión general** del producto durante el desarrollo.
Jeff Patton propone el enfoque de **User Story Mapping** como una forma de mantener esa visión clara.

---

### **Problema que expone:**

* Los equipos suelen enfocarse en **listas de funcionalidades (backlogs)** como si fueran listas de tareas.
* Esto lleva a productos **fragmentados**, difíciles de usar o que no resuelven bien los problemas del usuario.
* Se pierde la conexión entre las historias individuales y el **objetivo general del producto**.

---

### **¿Qué propone?**

* Utilizar un **mapa de historias de usuario (User Story Map)**, que muestra:

  * Las **actividades principales del usuario**.
  * Las **tareas específicas** que realiza.
  * El orden y contexto en que se usan.
* De esta manera, el equipo puede visualizar **todo el flujo del producto** y construir versiones útiles, coherentes y priorizadas.

---

### **Ejemplo:**

* Habla de una funcionalidad donde técnicamente todo estaba desarrollado, pero el producto **no era útil para el usuario final**.
* Resalta que la funcionalidad sin contexto **no genera valor**.

---

### **Frases clave del capítulo:**

* *“We get so focused on building the thing right, we lose sight of building the right thing.”*
* *“Software that’s delivered and not used is worse than no software at all.”*

---

### **Conclusión del capítulo:**

* Es vital **entender el panorama completo** antes de desarrollar.
* El **story mapping** ayuda a alinear a todo el equipo, priorizar entregas valiosas y mantener la visión centrada en el usuario.
* No se trata solo de entregar software, sino de entregar **impacto real**.

---

## **Capítulo 2: Plan to Build Less**

### **Idea principal:**

En lugar de construir todo lo posible, debemos **planificar construir menos**, enfocándonos en **entregar valor real** al usuario y aprendiendo con cada entrega.

---

### **Problemas que se plantean:**

* Los equipos suelen enfocarse en cumplir con un backlog completo como si fuera una lista de tareas.
* Esto lleva a productos con muchas funcionalidades, pero **sin utilidad real o con sobrecarga**.
* Asumir que más funcionalidades = más valor es una **falacia común**.

---

### **Solución propuesta:**

* Planificar **entregas pequeñas pero funcionales** (versiones mínimas utilizables).
* Priorizar lo que realmente permite **resolver problemas del usuario**.
* Usar mapas de historias para visualizar el flujo y **decidir qué construir primero**.

---

### **Conceptos clave:**

* **Release slices**: cortes verticales del producto que incluyen suficiente funcionalidad como para ser útiles.
* **Entregar temprano y aprender rápido**: cada versión permite obtener feedback y ajustar.
* **No es necesario construir todo para entregar valor.**

---

### **Frase destacada:**

> *“Plan to build less. Not more. Not everything.”*

---

### **Conclusión:**

* El verdadero objetivo no es completar el backlog, sino **resolver problemas reales con el menor esfuerzo posible**.
* El story mapping ayuda a planificar mejor y a construir **productos más enfocados y valiosos**.
