# 19. Explique a qué se hace referencia con el término “Estimación de costos”.

La estimación de costos es un conjunto de técnicas utilizadas para determinar cuánto tiempo, esfuerzo y perfiles de RRHH se necesitan para la construcción de un sistema de Software.

# 20. ¿Cuáles son las técnicas de estimación y para qué se utilizan?

* **Lluvia de ideas**: se generan ideas en grupo para conseguir soluciones creativas e innovadoras, buscando romper los paradigmas establecidos. El ambiente participativo asegura una mejor calidad en las decisiones tomadas por el grupo, más compromiso de los participantes en la actividad y un sentimiento de responsabilidad compartida.

* **Opinión de expertos**: usa la experiencia de algún desarrollador *senior* para describir los parámetros del proyecto y realizar predicciones basadas en experiencias previas.

* **Analogía**: el equipo de estimadores compara el nuevo proyecto con otros proyectos similares ya realizados. Consiste en identificar similitudes y diferencias para poder realizar la estimación. Es más simple y visible, pero exige definir las características claves que asemejan y diferencian a los proyectos.

* **Descomposición**: se descompone el producto en componentes y las actividades en tareas. Luego el análisis se focaliza en estas divisiones. La estimación se realiza en base a casos promedios o experiencias previas.
    * **Bottom-up:** se estima cada tarea de menor nivel y luego se unen para formar la estimación general.
    * **Top-down:** estima el proceso completo, y la estimación de cada componente se calcula como una porción relativa del todo.

# 21. El modelo COCOMO original es una colección de tres modelos (Básico, Intermedio y Avanzado/detallado). Explique las diferencias entre estos modelos.

Cada modelo se utiliza según el conocimiento que se tenga del proyecto o la etapa en la que este se encuentre:
1. El modelo **básico** es aplicable cuando se conoce muy poco del proyecto.
2. El modelo **intermedio** es aplicable luego de la especificación de requerimientos.
3. El modelo **avanzado** es aplicable una vez terminado el diseño.

# 22. Los modelos calculan el esfuerzo requerido E a través de una fórmula de la forma: $E = a * S^b * F$, y la duración estimada a través de la fórmula: $D = c * E^d$
## a. ¿Qué valor toma F para el modelo básico?

En el modelo básico, $F = 1$.

## b. Describir brevemente en función de qué tipos de variables se calcula el factor de ajuste F en los otros dos modelos.

Los factores de ajuste se pueden clasificar en:
* **Atributos del producto:** referidos al tamaño, riesgos y complejidad del producto.
* **Atributos del hardware:** referido a las limitaciones sobre los componentes en los que se ejecutará el producto en producción.
* **Atributos del personal:** referido a las capacidades y experiencia de los programadores u otro tipo de personal involucrado (por ejemplo, analistas funcionales).
* **Atributos del proyecto:** referido a las prácticas de software y al esfuerzo necesario para cumplir con la planificación.

## c. Indicar cómo varían los valores de a y b, y c y d en ambas fórmulas de acuerdo al modo utilizado.

Las fórmulas de Personas-Mes (PM) y de Tiempo de Desarrollo (TD) son las siguientes:

* $PM = a*(KDSI^b)$
* $TD = c*(PM^d)$

El valor de $KDSI$ se define como miles de líneas de código entregables.

Los valores de $a, b, c, d$ varían según la clasificación del sistema sobre el que se esté trabajando:

| Clasificación |  a   |  b   |  c   |  d   |
| ------------- | ---- | ---- | ---- | ---- |
| Orgánico      | 2.40 | 1.05 | 2.50 | 0.38 |
| Embebido      | 3.00 | 1.12 | 2.50 | 0.35 |
| Semi-embebido | 3.60 | 1.20 | 2.50 | 0.32 |

## d. Describir las características generales de sistemas que apliquen a cada uno de estos modos:

### Orgánico

Son sistemas generales cuyo principal foco es el software. Realizan operaciones de procesamiento, transacciones y recuperación de datos.

Ejemplos de este tipo de sistemas serían sistemas de facturación o generación de reportes.

### Embebido

Sistemas de software en tiempo real que se integran a un sistema mayor basado en hardware.

Ejemplos de este tipo de sistemas serían controladores de ascensores o semáforos.

### Semi-embebido

Combinación entre las clasificaciones previas. Son sistemas embebidos con alto número de transacciones que deben ser procesadas.

Ejemplos de este tipo de sistemas serían sistemas de monitoreo de red.

# 23. ¿Cuáles son los principales objetivos considerados en el desarrollo del modelo COCOMO 2.0? Explique diferencias con la versión original.

El principal motivo para una nueva versión de COCOMO es que éste no era aplicable a los entornos modernos de desarrollo. Los objetivos de COCOMO 2 son los siguientes:
* Desarrollar modelos de costos y estimación acordes a las prácticas actuales.
* Desarrollar bases de datos y herramientas que soporten la mejora continua del modelo.
* Proveer un *framework* analítico y cuantitativo, con un conjunto de herramientas y técnicas para evaluar los efectos de mejoras en los costos de ciclos de vida y planificaciones.

Esta nueva versión es más escalable y permite adaptarse a las nuevas tecnologías. También presenta más alternativas para la estimación de costos, basándose en líneas de código, Puntos Objeto o Puntos Función.

# 24. Explique qué es la economía de escala. De al menos dos ejemplos

La economía de escala indica el aumento de productividad a medida que aumente el tamaño del producto. En el caso de no presentarse, indica los retrasos producidos en el proyecto debido al aumento de tamaño en el producto.

En la estimación de costos de COCOMO 2, pueden darse 3 casos:
* El proyecto tiene economía de escala, por lo que su productividad aumenta con el tamaño del producto.
* La economía y no-economía de escala están balanceadas.
* El proyecto no presenta economía de escala, por lo que su productividad se ve reducida con el aumento de tamaño del producto.