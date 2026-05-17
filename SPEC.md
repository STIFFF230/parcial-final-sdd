# Especificación del sistema

Nombre del proyecto:
Calculadora de Nota Final Universitaria

Objetivo:
Crear una aplicación web que permita calcular cuánto necesita sacar un estudiante en la última nota para aprobar una materia con mínimo 3.0.

## Requerimientos funcionales

RF01. El sistema debe permitir ingresar el nombre de la materia.
RF02. El sistema debe permitir ingresar las notas ya obtenidas.
RF03. El sistema debe permitir ingresar el porcentaje de cada nota.
RF04. El sistema debe calcular la nota acumulada.
RF05. El sistema debe calcular cuánto necesita sacar el estudiante en la última nota para llegar a 3.0.
RF06. El sistema debe mostrar si el estudiante ya está aprobando.
RF07. El sistema debe mostrar si no es posible aprobar porque necesita más de 5.0.
RF08. El sistema debe validar que las notas estén entre 0.0 y 5.0.
RF09. El sistema debe validar que los porcentajes no superen el 100%.
RF10. El sistema debe permitir limpiar los campos.

## Requerimientos no funcionales

RNF01. La interfaz debe ser clara y fácil de usar.
RNF02. La aplicación debe ser responsive.
RNF03. Debe funcionar sin conexión a internet.
RNF04. El resultado debe mostrarse con dos decimales.
RNF05. Los mensajes de error deben ser claros.
RNF06. El código debe estar comentado.
RNF07. La aplicación debe ejecutarse desde un navegador.

## Reglas de cálculo

La nota final mínima para aprobar es 3.0.

La nota acumulada se calcula así:

nota_acumulada = suma de cada nota multiplicada por su porcentaje dividido entre 100

La nota necesaria se calcula así:

nota_necesaria = (3.0 - nota_acumulada) / (porcentaje_restante / 100)

Si la nota necesaria es mayor a 5.0, el sistema debe indicar que no es posible aprobar.