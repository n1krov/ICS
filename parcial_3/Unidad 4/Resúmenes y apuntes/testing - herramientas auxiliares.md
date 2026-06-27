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

# Herramientas auxiliares para las pruebas de software

En el contexto de las **pruebas de software**, especialmente en la **prueba de unidades** o **pruebas de integración incremental**, los **controladores (drivers)** y **stubs (resguardos)** son herramientas auxiliares que se utilizan cuando ciertas partes del sistema aún no están desarrolladas o disponibles. También se los conoce como **programas "simulados" o "representativos"**.

---

### ¿Qué son?

#### **Stubs (resguardos o sustitutos)**:

* Son **módulos simulados que reemplazan a componentes subordinados** aún no implementados.
* Simulan el **comportamiento de una función o procedimiento llamado** por la unidad en prueba.
* Devuelven **respuestas predefinidas** para ciertas llamadas, sin ejecutar la lógica real.
* Se usan en **pruebas descendentes** (top-down).

**Ejemplo**:
Supongamos que estás probando una función A que depende de la función B. Si B todavía no está lista, creás un stub de B que simplemente devuelve un valor fijo para que puedas seguir probando A.

---

#### **Drivers (controladores)**:

* Son **módulos simulados que llaman al componente en prueba**, actuando como programa principal.
* Son necesarios cuando la unidad que se quiere probar **es invocada por otras partes del sistema aún no desarrolladas**.
* Se usan en **pruebas ascendentes** (bottom-up).

**Ejemplo**:
Si la función C está lista pero nadie la llama directamente todavía (porque la función que la usa no está desarrollada), creás un driver que simula una llamada a C con ciertos valores para probarla.

---

### ¿Por qué se usan?

* Para permitir **pruebas tempranas**, incluso si el sistema aún no está completo.
* Para **aislar componentes** y probarlos en forma independiente.
* Para **detectar errores más fácilmente**, sin depender de otros módulos.

---

### Ejemplo concreto:

```plaintext
Función en desarrollo: calcularPromedio()
Dependencias:
  - leerNotas()   ← aún no implementada
  - mostrarResultado() ← aún no implementada

→ Stub de leerNotas(): retorna una lista fija de notas.
→ Stub de mostrarResultado(): imprime el resultado en consola.

→ Driver: crea un programa que llama a calcularPromedio() y muestra el resultado.
```

---

### Resumen

| Componente | Función                         | Uso principal         |
| ---------- | ------------------------------- | --------------------- |
| **Stub**   | Simula un módulo **invocado**   | Pruebas **top-down**  |
| **Driver** | Simula un módulo que **invoca** | Pruebas **bottom-up** |

