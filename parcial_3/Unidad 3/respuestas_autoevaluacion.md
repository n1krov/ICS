**1. Diferencia entre Scrum y XP**
XP es una disciplina de desarrollo centrada en prácticas técnicas de programación, mientras que Scrum es un marco de trabajo (framework) iterativo e incremental para la gestión general de proyectos de cualquier tipo.

**2. Antipatrones de XP**
*   **Retroalimentación al final:** Entregar el software recién al finalizar el proyecto, impidiendo la adaptación.
*   **Falta de coraje ("No tener huevos"):** Negarse a aceptar cambios trascendentales en etapas tardías.
*   **Complejidad:** Diseñar el sistema más complejo creyendo que es necesario para prever futuras funcionalidades.
*   **Sin pruebas (Prueban’t):** No realizar pruebas automatizadas y unitarias sobre el código desarrollado.
*   **Sin calidad (Calidan’t):** Negociar la calidad técnica y permitir que se acumule deuda técnica perjudicial.

**3. Características de una HU bien definida**
Deben centrarse en la conversación en lugar de la documentación y seguir el método **INVEST**: Independientes, Negociables, Valorables (aportar valor), Estimables, Pequeñas (Small) y Testeables.

**4. Bad Smell de una HU (Contraejemplo)**
*Stories are too small* (historias demasiado pequeñas).
Ejemplo: Separar "guardar resultados en XML" y "guardar resultados en HTML" en dos historias diferentes. Al ser tan pequeñas el trabajo se solapa. Esto causa graves problemas al estimar y planificar, ya que el esfuerzo real dependerá totalmente del orden en que se implementen.

**5. Por qué usar Historias de Usuario**
Porque priorizan la **colaboración y la conversación** cara a cara por encima de la documentación exhaustiva. Las HU aseguran una verdadera comprensión compartida, evitando el problema de los viejos requisitos donde lo escrito rara vez se interpreta igual por todos.

**6. Categorías del método MoSCoW**
Ejemplo para un sistema e-commerce:
*   **Must have (Debe tener):** Pasarela de pagos (crítico, sin esto el sistema no sirve).
*   **Should have (Debería tener):** Historial de compras del usuario (importante pero no crítico).
*   **Could have (Podría tener):** Sugerencias de productos relacionados (deseable si sobra tiempo).
*   **Won't have (No tendrá):** Pagos con criptomonedas (descartado para esta iteración).

**7. Definir un MVP**
Sirve para **mitigar riesgos** identificando de manera temprana si se comprenden las necesidades del usuario, entregando valor lo antes posible. Se hace agrupando el **software funcional mínimo**, que incluya al menos todas las historias prioritarias (Must have).

**8. Técnica de planning poker**
El Product Owner presenta una historia (ej. "Login"). Cada desarrollador elige en secreto una carta (con números no lineales como Fibonacci 1,2,3,5,8) que representa su estimación. Si todos muestran la misma carta, se acepta; si uno pone 2 y otro 8, discuten sus razones técnicas y repiten hasta alcanzar consenso.

**9. Punto historia y estimación**
Es una medida subjetiva que representa el **esfuerzo ideal** medido en tiempo (jornadas). Asume error porque los humanos somos malos estimando tiempos exactos a futuro, pero muy buenos **comparando cosas de forma relativa**. Se mejora utilizando datos históricos de sprints previos (velocidad) y manteniendo estable al equipo.

**10. Roles en el proceso de estimación**
El proceso lo realiza colaborativamente **el equipo de desarrollo**.

**11. Diferencias en estimación (ágil vs clásica)**
En las metodologías clásicas (cascada), se estima **todo el proyecto al inicio** usando métodos paramétricos (como líneas de código). En la agilidad, la estimación es iterativa, utilizando métodos **heurísticos y comparación relativa**, enfocándose sólo en lo priorizado del sprint.

**12. Prioridad al estimar**
Se debe priorizar siempre **lo que aporta valor de negocio / lo que el cliente necesita**, determinado por el Product Owner, no la facilidad técnica ni los costos de las actividades.

**13. Historias casi terminadas**
No suman. Para que una historia se considere terminada debe cumplir obligatoriamente el acuerdo del **Definition of Done (DoD)**. Una historia al 90% no cumple el DoD, por lo que no está terminada y aporta cero puntos a la velocidad.

**14. Cuándo hacer un Mapa de HU**
Debe hacerse al **principio del proyecto** para captar la visión general del producto, y luego modificarse **constantemente** durante el desarrollo, ya que funciona como el Product Backlog vivo.

**15. El método INVEST y la calidad**
Sí, el acrónimo INVEST es el criterio principal y guía utilizada específicamente para **asegurar la correcta calidad** y definición al escribir historias de usuario.

**16. Práctica de XP**
**Programación en parejas (Pair Programming):** Todo el código se escribe entre dos programadores en una misma computadora. Uno se concentra en la codificación y los detalles (el que usa el teclado), mientras el otro revisa constantemente y piensa en la estrategia de diseño general.

**17. Pilares de Scrum**
**Transparencia, Inspección y Adaptación**.
Ejemplo de Adaptación: Si durante una iteración el equipo nota que un proceso o tecnología está desviándose o generando errores graves, se ajusta el plan inmediatamente para cambiar el rumbo y evitar el fracaso.

**18. Encargado del Product Backlog**
El único encargado de mantenerlo, ordenarlo y priorizarlo es el **Product Owner**.

**19. Roles de Scrum**
Scrum Master, Product Owner y Equipo de Desarrollo.
**El Product Owner:** Es el representante del negocio, encargado de maximizar el valor del producto y de gestionar, traducir y priorizar todas las necesidades del cliente en el Product Backlog.

**20. Equipo autónomo, adaptable y responsable**
Son **autogestionados** (deciden internamente quién, cómo y cuándo ejecuta las tareas), responden con flexibilidad ante los cambios y asumen la toma de decisiones por consenso de forma que son responsables directos de los resultados.

**21. Características de las Dailys**
Son reuniones diarias breves de máximo **15 minutos**, siempre en el mismo horario y lugar. Se responde ¿qué hice ayer?, ¿qué haré hoy? y ¿qué problemas tengo?, enfocándose únicamente en informar el progreso sin entrar en debates profundos.

**22. Meeting de Scrum (Ejemplo)**
**Sprint Review:** Intervienen el Equipo, PO, Scrum Master y Stakeholders (usuarios) al final de cada sprint. Se realiza para presentar la demo del *software funcionando* (incremento), recibir feedback del cliente y validar si se cumplieron los objetivos del negocio.

**23. Medición del avance**
El avance se mide evaluando el **software funcionando** real entregado (working SW) y controlando el **trabajo pendiente** a través de gráficos como el *Burn-down*.

**24. Características del equipo en Scrum**
Deben ser **Multifuncionales** (con todas las capacidades técnicas necesarias), **Autogestionados** y **Pequeños** (idealmente de 3 a 7 personas).

**25. DoD (Definition of Done)**
Es un acuerdo o **lista de condiciones de calidad** que una historia de usuario debe superar para considerarse completamente terminada. Se acuerda entre el PO y el equipo de desarrollo **antes de comenzar a estimar**.

**26. Contraposición de Kent Beck (Costo y Cambio)**
Tradicionalmente (Boehm), se asume que el costo del cambio crece exponencialmente con el tiempo. Kent Beck propone que, usando agilidad (pruebas y diseño simple), **la curva se aplana**, haciendo que el costo de introducir un cambio permanezca estable sin importar cuándo ocurra.

**27. Ejemplo en Spotify**
*   **HU:** Como usuario, quiero agregar una canción a mi playlist para mantenerla actualizada.
*   **Tareas:** Programar botón UI, armar lógica backend en Base de Datos, crear pruebas.
*   **DoD:** Pruebas automáticas aprobadas y validación final del PO.
*   **Criterios de aceptación:** 1) La canción debe verse en la playlist inmediatamente. 2) Se refleja el guardado en la base de datos.

**28. Sprint Backlog vs Product Backlog**
El **Product Backlog** es la lista total, emergente y ordenada por valor de todo lo necesario para el producto (gestionada por el PO). El **Sprint Backlog** es el subconjunto de esos ítems seleccionados exclusivamente por el equipo de desarrollo para ejecutar en la iteración actual.

**29. Medición del avance en SCRUM**
A través del **software en funcionamiento** entregado y el control del conjunto de historias que disminuye (el **trabajo pendiente**) visualizado en el *burn-down chart*.

**30. Scrum solo con el equipo y Scrum Master**
Faltaría el rol del **Product Owner**, por lo que el proyecto no tendría dirección comercial. El equipo no sabría qué construir primero porque faltarían los requisitos priorizados por valor del negocio, arriesgándose a crear un sistema técnico impecable pero que no cumpla las necesidades del cliente.

**31. Característica exclusiva de Kanban**
Los **Límites de Trabajo en Progreso (WIP Limits)**. Kanban establece un cupo máximo estricto para las tareas en curso en cada columna, lo que evita la sobrecarga, gestiona los cuellos de botella y crea un sistema *pull* (el trabajo avanza solo cuando hay capacidad libre).

**32. Planificación en técnicas ágiles**
**Se planifica el doble.** A diferencia de los métodos tradicionales, donde se hace una planificación estricta solo al principio, en los enfoques ágiles se reevalúa y reajusta la planificación de forma iterativa y continua (por ejemplo, en cada *Sprint Planning*). Se supervisan y planifican los próximos pasos constantemente a medida que se aprende más sobre el proyecto y se adaptan a los cambios.

**33. Relaciones entre Scrum y XP**
*   **Coraje (Valor):** Ambas aplican el valor del coraje para aceptar desafíos complejos, desechar código malo o modificar requisitos tardíos.
*   **Abrazar el cambio (Principio):** Las dos metodologías basan su éxito en el empirismo y en la capacidad constante de adaptarse a la evolución de las necesidades.
*   **Entregas iterativas (Práctica):** XP lo hace con "lanzamientos pequeños" y Scrum con incrementos continuos al final de cada "Sprint".