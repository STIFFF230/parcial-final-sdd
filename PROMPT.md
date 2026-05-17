# Prompt utilizado

IA utilizada:
ChatGPT

Prompt:

Actúa como un ingeniero de software experto en Spec Driven Development. Necesito que desarrolles una aplicación web sencilla llamada “Calculadora de Nota Final Universitaria”, siguiendo estrictamente los requerimientos especificados.

Primero interpreta la especificación, luego genera la solución completa en un solo archivo HTML que incluya HTML, CSS y JavaScript interno. La aplicación debe funcionar sin backend, sin instalación de librerías externas y debe poder ejecutarse abriendo el archivo index.html en un navegador.

ESPECIFICACIÓN DEL SISTEMA

Objetivo:
Crear una aplicación web que permita a un estudiante calcular cuánto necesita sacar en la última nota de una materia para alcanzar una nota final mínima de 3.0.

Requerimientos funcionales:
RF01. El sistema debe permitir ingresar el nombre de la materia.
RF02. El sistema debe permitir ingresar las notas ya obtenidas.
RF03. El sistema debe permitir ingresar el porcentaje de cada nota ya obtenida.
RF04. El sistema debe permitir ingresar el porcentaje que falta por evaluar.
RF05. El sistema debe calcular automáticamente la nota acumulada.
RF06. El sistema debe calcular cuánto necesita sacar el estudiante en la última nota para llegar a 3.0.
RF07. Si el estudiante ya alcanza 3.0 con las notas actuales, el sistema debe mostrar un mensaje indicando que ya va aprobando.
RF08. Si la nota necesaria es mayor a 5.0, el sistema debe mostrar un mensaje indicando que no es posible alcanzar 3.0 solo con la nota restante.
RF09. El sistema debe validar que las notas estén entre 0.0 y 5.0.
RF10. El sistema debe validar que los porcentajes no superen el 100%.
RF11. El sistema debe mostrar el resultado de forma clara, incluyendo materia, nota acumulada, porcentaje evaluado, porcentaje restante y nota necesaria.
RF12. El sistema debe tener un botón para limpiar todos los campos.

Requerimientos no funcionales:
RNF01. La interfaz debe ser sencilla, clara y fácil de usar.
RNF02. El diseño debe ser responsive para verse bien en computador y celular.
RNF03. El código debe estar comentado en las partes principales.
RNF04. La aplicación debe funcionar sin conexión a internet.
RNF05. El cálculo debe redondearse a dos decimales.
RNF06. El sistema debe mostrar mensajes de error comprensibles para el usuario.
RNF07. El diseño debe tener estilo visual moderno, con tarjetas, botones claros y colores suaves.

Reglas de cálculo:
1. La nota final mínima para aprobar es 3.0.
2. La nota acumulada se calcula multiplicando cada nota por su porcentaje y dividiendo entre 100.
3. La nota necesaria se calcula así:
nota_necesaria = (3.0 - nota_acumulada) / (porcentaje_restante / 100)
4. Si porcentaje_restante es 0, el sistema debe indicar que no hay porcentaje pendiente por evaluar.
5. Si la suma de porcentajes supera 100%, debe aparecer un error.

Pruebas que debe incluir la respuesta:
Después del código, incluye una sección llamada “Pruebas de validación”, donde expliques al menos 5 casos de prueba:
1. Caso normal donde sí se puede aprobar.
2. Caso donde ya va aprobando.
3. Caso donde necesita más de 5.0.
4. Caso con porcentajes mayores a 100%.
5. Caso con nota fuera del rango permitido.

Formato de respuesta:
1. Explica brevemente cómo la solución sigue el enfoque Spec Driven Development.
2. Entrega el código completo del archivo index.html.
3. Entrega las pruebas de validación.
4. Entrega un análisis corto indicando qué requerimientos se cumplieron y qué se podría mejorar.