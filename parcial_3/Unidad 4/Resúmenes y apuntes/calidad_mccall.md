---
title: "Ingeniería y Calidad de Software"
author: "Suzy Suicidio"
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
  - \usepackage{longtable}
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

# Factores de Calidad según McCall

## Introducción

Jim McCall propuso un modelo para evaluar la calidad del software basado en **factores**, **criterios** y **métricas**, con el objetivo de poder medirla de forma **objetiva y estructurada**. Su enfoque se organiza en **tres niveles de análisis** y agrupa los factores en **tres grandes categorías funcionales** del software.

---

## Categorías de los Factores de Calidad

Los **factores de calidad** según McCall se agrupan en tres grandes **categorías**, como se representa en el siguiente triángulo:

![Factores de calidad](factores_de_calidad.png)

### 1. Operación del Producto

Evalúa cómo se comporta el software desde el punto de vista del **usuario final** durante su ejecución.

**Factores incluidos:**

* Corrección
* Confiabilidad (Fiabilidad)
* Usabilidad
* Integridad
* Eficiencia

---

### 2. Revisión del Producto

Evalúa la **capacidad del software de ser modificado, corregido o mejorado** durante su mantenimiento o evolución.

**Factores incluidos:**

* Facilidad de recibir mantenimiento
* Flexibilidad
* Susceptibilidad de someterse a pruebas (testabilidad)

---

### 3. Transición del Producto

Evalúa la **capacidad del software de adaptarse a diferentes entornos tecnológicos o aplicaciones futuras**.

**Factores incluidos:**

* Portabilidad
* Reusabilidad
* Interoperabilidad

---

## Proceso de Evaluación de la Calidad del Software

McCall propone **tres niveles jerárquicos** para medir la calidad del software:

### Paso 1: Factores de Calidad

Se identifican los **atributos generales** del software que se desean evaluar (como los mencionados en las categorías anteriores). Estos factores definen **qué** queremos medir.

Ejemplo: Usabilidad, Fiabilidad, Portabilidad.

---

### Paso 2: Criterios del Producto

Cada factor se descompone en **criterios observables**, que permiten analizar más específicamente el comportamiento o características del producto.

Ejemplo: Para "Usabilidad", uno de los criterios puede ser la **facilidad de aprendizaje**.

---

### Paso 3: Métricas del Producto

Se definen **indicadores cuantitativos** que permiten medir objetivamente cada criterio.

Ejemplo: Tiempo promedio (en minutos) que tarda un usuario nuevo en completar una tarea básica.

---

## Esquema Resumido

```text
FACTOR → CRITERIO → MÉTRICA
```

**Ejemplo aplicado:**

* Factor: Usabilidad
* Criterio: Facilidad de aprendizaje
* Métrica: Tiempo medio en minutos para completar una operación típica por usuarios nuevos

---

## Conclusión

El modelo de McCall permite abordar la calidad del software de forma **estructurada y medible**, facilitando su mejora continua a través de datos concretos. Cada factor de calidad no debe analizarse de manera subjetiva, sino mediante criterios claros y métricas asociadas que guíen las decisiones del equipo de desarrollo y mantenimiento.

---

# Ejemplo Aplicado: App Bancaria Móvil

Imaginemos que queremos evaluar la **calidad de una aplicación móvil de banca online** desarrollada por una entidad financiera. Aplicamos los tres pasos del modelo de McCall:

## **Paso 1: Factor de calidad**

**Usabilidad**:

Queremos que los usuarios puedan operar la app de forma sencilla, sin necesidad de entrenamiento ni errores frecuentes.

---

## **Paso 2: Criterio del producto**

**Facilidad de aprendizaje**:

Evaluamos qué tan fácil es para un nuevo usuario completar una tarea básica, como realizar una transferencia.

---

## **Paso 3: Métrica del producto**

**Tiempo promedio (en minutos)**, que tardan 10 usuarios nuevos en completar su primera transferencia bancaria sin ayuda externa.

Supongamos que se mide en un test de usuario y el valor promedio obtenido es **4,2 minutos**.

---

## Otro ejemplo adicional:

\begin{longtable}{|>{\centering\arraybackslash}p{3.5cm}|>{\centering\arraybackslash}p{4cm}|>{\centering\arraybackslash}p{7cm}|}
\hline
\textbf{Factor} & \textbf{Criterio} & \textbf{Métrica} \\
\hline
Fiabilidad & Tolerancia a fallos & Porcentaje de operaciones completadas correctamente tras una desconexión de red \\
\hline
Portabilidad & Adaptabilidad & Número de cambios requeridos para que la app funcione en iOS además de Android \\
\hline
\end{longtable}

---

Este tipo de evaluación permite al equipo de desarrollo **tomar decisiones basadas en evidencia**, como rediseñar interfaces, mejorar documentación o fortalecer pruebas, para alcanzar los niveles de calidad deseados.

---
