# Prompt utilizado

IA utilizada: Claude
Plan utilizado: Claude de pago

## Prompt único enviado a la IA

Actúa como un ingeniero de software experto en Spec Driven Development (SDD).

CONTEXTO DEL PROYECTO:
Este proyecto se llama "parcial-final-sdd" y está conectado desde mi repositorio de GitHub. Contiene los siguientes archivos:

- SPEC.md → Especificación del sistema con requerimientos funcionales (RF), no funcionales (RNF) y reglas de cálculo.
- PROMPT.md → Documento donde está registrado el prompt original utilizado.
- README.md → Descripción general del proyecto.
- ANALISIS.md → Análisis del resultado.
- index.html → Archivo donde DEBE quedar la solución completa (actualmente está vacío).

TU TAREA:
1. Lee primero el archivo SPEC.md del repositorio. Esa es la fuente de verdad del proyecto.
2. Lee también PROMPT.md para entender el contexto adicional.
3. A partir de la especificación, genera la solución completa de la aplicación web llamada "Calculadora de Nota Final Universitaria".
4. Toda la solución debe ir en UN SOLO archivo llamado index.html que contenga HTML, CSS y JavaScript internos (sin librerías externas, sin backend, sin dependencias).
5. La aplicación debe ejecutarse abriendo index.html directamente en un navegador, incluso sin conexión a internet.

REQUISITOS DE CUMPLIMIENTO:
- Implementa TODOS los requerimientos funcionales (RF) definidos en SPEC.md.
- Implementa TODOS los requerimientos no funcionales (RNF) definidos en SPEC.md.
- Aplica las reglas de cálculo exactamente como están especificadas:
  * nota_acumulada = suma de (nota * porcentaje / 100)
  * nota_necesaria = (3.0 - nota_acumulada) / (porcentaje_restante / 100)
  * Nota mínima para aprobar: 3.0
  * Si nota_necesaria > 5.0 → mostrar que no es posible aprobar
  * Si el estudiante ya alcanza 3.0 → mostrar que ya va aprobando
- Validaciones obligatorias:
  * Notas entre 0.0 y 5.0
  * Porcentajes que no superen 100% en total
  * Mensajes de error claros para el usuario
- Resultados con 2 decimales.
- Diseño responsive (computador y celular).
- Código comentado en las partes principales.
- Estilo visual moderno con tarjetas, botones claros y colores suaves.

FORMATO DE TU RESPUESTA:
1. Primero, una breve explicación (máximo 5 líneas) de cómo tu solución sigue el enfoque Spec Driven Development.
2. Luego, el código completo del archivo index.html dentro de un bloque de código.
3. Después, una sección llamada "Pruebas de validación" con al menos 5 casos de prueba:
   - Caso 1: estudiante que sí puede aprobar (caso normal).
   - Caso 2: estudiante que ya va aprobando.
   - Caso 3: estudiante que necesita más de 5.0 (imposible).
   - Caso 4: porcentajes que suman más de 100%.
   - Caso 5: nota fuera del rango permitido.
4. Finalmente, una sección llamada "Análisis de cumplimiento" donde indiques qué requerimientos del SPEC.md se cumplen y cuáles se podrían mejorar.

IMPORTANTE:
- No me pidas confirmación ni hagas preguntas adicionales. Genera la solución completa en una sola respuesta.
- El código debe estar listo para copiar y pegar en index.html sin modificaciones.
- Si encuentras ambigüedades en SPEC.md, decide tú mismo la mejor implementación y explica brevemente por qué en el análisis final.
