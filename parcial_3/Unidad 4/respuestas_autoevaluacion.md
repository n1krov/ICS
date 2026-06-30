**1.** La calidad es el conjunto de propiedades y características inherentes de un producto o servicio que le confieren su aptitud para satisfacer las necesidades explícitas o implícitas del cliente.

**2.** La calidad depende fundamentalmente de las necesidades de las personas, basándose de manera específica en lo que el usuario quiere y en cómo lo quiere.

**3.** Un producto de software posee calidad si provee valor y satisfacción a los usuarios, produce ganancias, genera pocas quejas y contribuye activamente a los objetivos de calidad de la organización.

**4.** Existe una fuerte relación: si un proceso no tiene calidad, es muy probable que el producto tampoco la tenga. Sin embargo, un proceso de calidad ayuda al producto, pero no lo garantiza al 100% porque interviene un tercer componente clave, que es el equipo.

**5.** Para asegurar la calidad del software se deben sumar integralmente tres aspectos: la calidad del proceso, la calidad del producto y la calidad de las personas.

**6.** La verificación evalúa si el producto se está construyendo correctamente, como al analizar la complejidad del código fuente. La validación confirma si se está construyendo el producto correcto para el mercado, usando como ejemplo las pruebas de aceptación de usuario.

**7.** Hacer software de baja calidad genera deuda técnica, lo que afecta gravemente la mantenibilidad y obliga al equipo a dedicar su tiempo a corregir errores en lugar de avanzar. Esto causa que la productividad del equipo caiga drásticamente, los costos suban, el personal se agote por el exceso de trabajo y el producto final sea rechazado por el mercado.

**8.** McCall divide la calidad estructuralmente en factores, criterios y métricas. Un ejemplo de factor es la "Fiabilidad" (la capacidad del sistema de no fallar), la cual se evalúa mediante criterios como la consistencia, exactitud y tolerancia a fallos.

**9.** La calidad no se añade en una fase exclusiva o final, sino que se incorpora continuamente en el software a lo largo de todo el proceso de ingeniería, desde que se comienza a pensar en el producto.

**10.** La verificación de la calidad debe realizarse constantemente a lo largo del proceso mediante pruebas. Las pruebas actúan como el último bastión para confirmar la calidad que ya debió construirse previamente en el software.

**11.** Las características de calidad en las personas incluyen el compromiso, la madurez técnica, la proactividad y el nivel de motivación o "engagement". Esto es vital porque el software lo hacen personas, y su nivel técnico y motivacional determina el éxito del proyecto y la calidad del producto final.

**12.** Un buen equipo debe ser maduro, aplicar constantemente buenas prácticas de ingeniería y ejecutar actividades de prueba desde el primer hasta el último día del sprint. Además, deben ser capaces de saldar la deuda técnica compartiendo la responsabilidad de forma colectiva.

**13.** Se observan dos niveles según el grado de involucramiento: el nivel transaccional, donde el personal es pasivo y se limita a hacer lo que se le pide, y el nivel transformacional, donde las personas muestran proactividad, crecimiento, impacto y un alto "engagement".

**14.** La principal consecuencia es la pérdida económica debido al impacto de la deuda técnica mala. Genera sistemas inmanejables, caídas severas de productividad por la constante corrección de errores, equipos agotados y pérdida de oportunidades en el mercado.

**15.** La deuda técnica es el aumento del costo y esfuerzo que supone trabajar en el presente con código inmaduro, deficiente o mal diseñado. En agilidad, se utiliza asumiendo a veces una pequeña deuda controlada para acelerar el desarrollo, siempre bajo el compromiso ineludible de pagarla rápidamente mediante refactorizaciones.

**16.** La deuda técnica "buena" es controlada y el equipo es plenamente consciente de ella para cumplir una entrega, planificando su corrección inmediata. La deuda técnica "mala" surge de la ignorancia o falta de calidad, es inconsciente, no se gestiona y destruye la productividad del equipo.

**17.** Ejemplo de deuda buena: pedir un préstamo bancario con cuotas calculadas para comprar herramientas que te darán ganancias inmediatas para pagar el crédito. Ejemplo de deuda mala: endeudarse sin control con la tarjeta de crédito por ignorancia, pagando altos intereses que te llevan a la quiebra.

**18.** Un tema fundamental relacionado con la calidad es el Pipeline de Integración Continua (IC) y Entrega Continua. Estas prácticas ayudan a ver la calidad automatizando la compilación, las pruebas y las inspecciones de código, mejorando la visibilidad del estado del proyecto.

**19.** El Aseguramiento de Calidad (QA) me asegura, mediante actividades preventivas, proactivas y de auditoría de los procesos, la confianza plena de que el producto final cumplirá con los requisitos de calidad esperados.

**20.** Los modelos de calidad de software son marcos de trabajo y estándares internacionales que establecen métodos, normas y métricas para guiar la adquisición, desarrollo, evaluación y mejora continua de los procesos y productos.

**21.** Los niveles de CMMI son: Incompleto (0), Ejecutado (1), Gestionado (2), Definido (3), Cuantitativamente gestionado (4) y Optimizando (5). El nivel 2 (Gestionado), por ejemplo, significa que el proceso se ejecuta con éxito y, además, se planifica, revisa y evalúa documentadamente para cumplir requisitos.

**22.** Para la calidad del proceso se utilizan modelos como CMMI, ISO 15504 (SPICE) e ISO 33000. Para la calidad del producto se emplean modelos como ISO 9126 y la serie ISO 25000 (SQuaRE).

**23.** QA (Aseguramiento) es un proceso preventivo enfocado en definir estrategias y procesos para evitar defectos, mientras que QC (Control) es un proceso reactivo enfocado en ejecutar pruebas para detectar defectos en el producto. No se puede hacer solo uno, ya que ambos se complementan: la gestión define la estrategia, QA vigila que se aplique, y QC ejecuta las pruebas concretas.

**24.** La técnica de caja blanca examina el código fuente interno y sus rutas lógicas, por ejemplo, probando todos los caminos independientes dentro de una estructura `while`. La técnica de caja negra trata al sistema como un bloque cerrado y evalúa solo entradas y salidas funcionales, por ejemplo, probar si un formulario rechaza una contraseña inválida.

**25.** Una técnica de prueba (ej. caja blanca) proporciona la herramienta o método específico para diseñar un caso de prueba concreto. Una estrategia de prueba es la guía de planificación que describe los pasos globales, indicando en qué momento, fase y con qué esfuerzo se desplegarán esas técnicas.

**26.** Las pruebas de Validación verifican puntualmente que el software cumpla todos los requerimientos funcionales y expectativas directas del cliente. Las pruebas de Sistemas combinan el software validado con otros elementos (como hardware, bases de datos o estrés de usuarios) para verificar el rendimiento global de todo el entorno operativo.

**27.** Test Coverage (Cobertura de prueba) es una métrica que indica la proporción o cantidad de código fuente del sistema que está siendo ejecutado y cubierto por los casos de prueba automatizados.

**28.** Deberían ejecutarse y escribirse *antes* de la codificación, sirviendo de esta forma como especificaciones ejecutables que guían el desarrollo, apoyando enfoques clave como TDD (Desarrollo Guiado por Pruebas).

**29.** Las pruebas de Unidad prueban componentes aislados y corresponden a la fase de Codificación. Las pruebas de Integración verifican la interacción entre módulos y se alinean con la fase de Diseño. Las pruebas de Validación comprueban el cumplimiento de requisitos del cliente y corresponden al Análisis. Las pruebas de Sistemas evalúan todo el conjunto y corresponden a la Ingeniería de Sistemas.

**30.** Una buena prueba no debe ser redundante y debe tener una alta probabilidad de encontrar un error, ya que su objetivo principal es destrozar el software. Además, no debe ser ni muy simple ni demasiado compleja, y debe ser "la mejor de la camada" para detectar clases completas de fallos optimizando recursos.

**31.** El testing automatizado (TA) consiste en la práctica de construir scripts o código que ejecuta pruebas sobre el software por sí mismo y se dispara mediante eventos preestablecidos en servidores de Integración Continua. Permite evitar que los errores afecten a los usuarios y ofrece confianza y agilidad para refactorizar.

**32.** No, el testing manual no desaparece por completo. El TA asume la carga de las pruebas repetitivas, estáticas o de regresión, permitiendo que el costoso esfuerzo humano se dedique a tareas de mayor valor, como las pruebas cualitativas de facilidad de uso y las pruebas exploratorias.

**33.** *(Nota: Esta información es externa a los apuntes dados, por lo que te sugiero verificarla independientemente)*. La IA Generativa puede incorporarse en el proceso de testing generando rápidamente conjuntos de datos masivos (mocks) para pruebas, autocompletando o sugiriendo casos de prueba unitarios en el IDE del programador, y proponiendo variaciones para pruebas de análisis de valores límite y partición equivalente basadas en las Historias de Usuario documentadas.