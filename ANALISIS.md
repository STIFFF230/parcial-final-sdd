# Análisis del resultado

El desarrollo realizado cumple con el enfoque de Spec Driven Development, porque antes de generar el código se definieron los requerimientos funcionales, no funcionales y las reglas de cálculo en el archivo SPEC.md. A partir de esa especificación se construyó el prompt entregado a la IA Claude, que generó la solución completa en un solo archivo HTML con HTML, CSS y JavaScript integrados.

La solución permite ingresar el nombre de la materia, las notas obtenidas, los porcentajes correspondientes y calcular cuánto necesita el estudiante en la última nota para aprobar con una nota mínima de 3.0. También incluye validaciones para evitar errores, como notas fuera del rango permitido o porcentajes que superan el 100%.

Después de probar la aplicación, se evidencia que cumple con la mayoría de los requerimientos planteados. Los casos normales funcionan correctamente, el sistema informa cuando el estudiante ya va aprobando y también muestra cuando no es posible aprobar porque se necesitaría una nota superior a 5.0. Adicionalmente, el cálculo se presenta con dos decimales y la interfaz es responsive, lo cual cubre los requerimientos no funcionales más relevantes.

Como mejora, se podría agregar una opción para guardar varias materias, exportar los resultados en PDF o almacenar los cálculos en el navegador usando LocalStorage. También se podría crear una versión con backend y base de datos, pero para el alcance del parcial la solución actual es adecuada porque es simple, funcional y verificable frente a la especificación inicial.
