# 13. Explique qué es Work Breakdown Structure (WBS) y cómo se construye.

Un WBS es una estructura jerárquica del trabajo que debe realizarse para completar el proyecto. El trabajo se divide en actividades, las cuales a su vez se dividen en tareas.

La construcción del WBS depende del líder del proyecto, y puede realizarse siguiendo dos enfoques:
* **Top-down:** se comienza a partir de la meta del proyecto (nivel 0), y comienza a dividirse en actividades. Según el nivel de participación del equipo, a su vez puede dividirse en:
    * **Equipo completo:** todo el equipo participa en la partición en todos los niveles que se considere adecuado. Una vez definidas las actividades, se decide cuáles deben secuencializarse y cuáles pueden ejecutarse concurrentemente.
    * **En sub-equipos:** el equipo completo define la partición de primer nivel, pero luego cada sub-equipo toma una actividad y se encarga de particionarla hasta el último nivel.
* **Bottom-up:** comienza con el equipo completo particionando el nivel 0, y luego se asigna cada actividad a un sub-equipo; estos intentarán dividirla en la mayor cantidad posible de tareas. Una vez divididas, se intentan agrupar en sub-actividades según su relación. Por último, vuelven a reunirse todos los equipos para discutir los resultados en conjunto. Este enfoque trae problemas respecto a la granularidad de las tareas.

# 14. Mencione los distintos usos del WBS en la administración de proyectos.

Las ventajas de usar un WBS son:
* Mejora la planificación del proyecto al momento de estimar esfuerzos, tiempos y recursos.
* Permite diseñar una arquitectura en base a actividades relacionadas.
* Facilita la administración del trabajo del proyecto.
* Genera informes sobre el estado y avance del proyecto.

# 15. Indique cuáles son las características que deben tener las actividades para considerarse completas. Explique.

1. **Estado medible:** en cualquier momento debe poder determinarse en qué estado se encuentra la actividad.
2. **Acotada:** debe poseer un evento de comienzo y un evento de fin. Generalmente determinado por fechas.
3. **Producir un entregable:** el entregable funciona como un signo visible de que la actividad se completó. Este puede ser un producto, un documento, una autorización para la próxima tarea, etc.
4. **Tiempo y costo medibles:** el tiempo y el costo deben ser fácilmente estimables. Realizar estas estimaciones para tareas de menor nivel permite calcular más fácilmente el total del proyecto.
5. **Duración aceptable:** considerando que hay excepciones, una actividad no debería trabajarse más de 2 semanas laborales.
6. **Independiente:** la independencia entre actividades permite que puedan realizarse sin interrupciones o esperar un recurso adicional. El esfuerzo dedicado a una actividad debe ser continuo.

# 16. Explique qué es la duración de una actividad. Indique cuál es la diferencia con el esfuerzo de trabajo.

La duración se define como el tiempo transcurrido en días laborales para finalizar el proyecto.

El esfuerzo de trabajo es la labor requerida para completar un trabajo, independientemente de que se realice de forma consecutiva.

Si bien al considerar la duración de una tarea se tiene en cuenta el esfuerzo de trabajo, también se consideran los imprevistos o interrupciones que podrían afectar los tiempos de entrega. Se podría considerar al esfuerzo de trabajo como el "tiempo neto" de labor dentro de la duración.

# 17. ¿Cuáles son las causas de variación en la duración de una actividad?

La duración de una actividad puede varias por distintas causas:

1. **Variaciones en los perfiles:** siempre se intenta asignar a la actividad a la persona más hábil para resolver ese tipo de problemas. Según la experiencia de la persona, la duración puede aumentar o reducirse.
2. **Eventos inesperados:** problemáticas externas que afectan al desarrollo. Esto pueden ser demoras de proveedores, problemas técnicos, enfermedades, etc.
3. **Eficiencia:** cuando un trabajador es interrumpido, su nivel de productividad se ve afectado y puede tardar en volver a su normalidad. Hay quienes se ven más afectados que otros, por lo que es importante conocer cómo mantener eficientes a los miembros del personal.
4. **Errores y malentendidos:** problemas en la comunicación que implican rehacer partes del trabajo.

# 18. Mencione las distintas técnicas para estimar esfuerzo.

* **Similitud con otras actividades:** se calcula la duración en base a las estimaciones ya realizadas en actividades similares para otros proyectos. Las personas que realizaron dichas actividades realizan la asociación y en base a eso estiman la nueva tarea.
* **Datos históricos:** similar al anterior, pero la organización mantiene un registro a partir del cual realizar la nueva estimación sin depender de lo que recuerde el personal.
* **Juicio experto:** realizadas por consultores expertos o vendedores con experiencia en las metodologías y tecnologías utilizadas. Estas estimaciones pueden no ser objetivas.
* **Técnica Delphi:** técnica grupal que crea una estimación a partir del conocimiento del grupo.
    * **Primera pasada:** cada persona le da un número de dificultad a la actividad.
    * **Segunda pasada:** quienes queden en los extremos (mayor-menor número) deben justificar su especificación. Luego de esto, los miembros vuelven a estimar y a partir de los nuevos resultados vuelven a justificarse.
    * **Tercera pasada:** se hace una última estimación y el promedio de esta pasada se usa como estimación del grupo.
* **Técnica de tres puntos:** se realiza una estimación para cada uno de estos escenarios: optimista (todo sucede acorde a lo planeado), media (duración usual) y pesimista (todo lo que puede fallar, falla). Luego, se toma el resultado de cada escenario y a partir de una fórmula se calcula la estimación general.
    
    $Estimación = (Optimista + 4*Media + Pesimista) / 6$
    
* **Técnica Delphi de banda ancha:** combina la técnica Delphi con la de 3 puntos. Cada integrante realiza las 3 estimaciones (optimista, media y pesimista), se recopilan los resultados y se eliminan los extremos. Luego se calcula el promedio para cada escenario y se calcula la estimación usando la fórmula de la técnica de 3 puntos.