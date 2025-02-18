# Arquitectura2S
Santiago:
1. Introduccion:
La Ley de Benford, también conocida como la ley de los primeros dígitos, es un fenómeno estadístico que describe la frecuencia con la que los dígitos ocurren en diversas colecciones de datos. A pesar de su aparente simplicidad, esta ley desafía la intuición, ya que sostiene que en muchos conjuntos de datos del mundo real, los números que comienzan con el dígito 1 aparecen con más frecuencia que los números que comienzan con el 2, y estos a su vez son más frecuentes que los que comienzan con el 3, y así sucesivamente. 

Esta distribución de dígitos no es aleatoria, sino que sigue una proporción logarítmica: aproximadamente el 30% de los números en un conjunto de datos empiezan con el dígito 1, el 17.6% con el 2, el 12.5% con el 3, y así en descenso. La ley fue observada por primera vez por el matemático Frank Benford en 1938, aunque ya había sido descrita anteriormente por Simon Newcomb en 1881. 

La Ley de Benford ha encontrado aplicaciones en una variedad de campos, desde la contabilidad forense hasta la ciencia de datos debido a su capacidad para detectar irregularidades y fraudes, ya que los datos manipulados o falsificados tienden a mostrar una distribución de dígitos diferente a la esperada según esta ley.

Nicolas 
3. Ensamblador - Registros

Los registros son componentes clave en la arquitectura de un procesador y en el lenguaje ensamblador. Son pequeñas unidades de almacenamiento dentro del procesador que se utilizan para guardar datos temporalmente durante la ejecución de instrucciones. Estos datos pueden ser operandos para cálculos, direcciones de memoria, resultados intermedios, entre otros.

En la arquitectura ARM, hay varios tipos de registros:

1. Registros de propósito general*: Estos son los registros principales que se utilizan para almacenar datos y realizar operaciones aritméticas y lógicas. En ARM, estos registros se denominan R0, R1, R2, etc., y generalmente hay 16 registros de propósito general (R0 a R15).
2. Registros especiales*:
   - R13 (SP)*: El registro de puntero de pila (Stack Pointer) que apunta al tope de la pila.
   - R14 (LR)*: El registro de enlace (Link Register) que guarda la dirección de retorno de una subrutina.
   - R15 (PC)*: El registro de contador de programa (Program Counter) que contiene la dirección de la siguiente instrucción a ejecutar.
3. Registros de estado: Contienen información sobre el estado del procesador y de las operaciones que se están llevando a cabo. En ARM, el registro de estado principal es el **CPSR (Current Program Status Register)*, que incluye bits de condición, bits de control y otros indicadores importantes.

Ejemplo utilizacion de registros en un programa ensamblador ARM:

assembly
    MOV R0, #10        ; Mover el valor 10 al registro R0
    MOV R1, #20        ; Mover el valor 20 al registro R1
    ADD R2, R0, R1     ; Sumar los valores de R0 y R1, y guardar el resultado en R2
    STR R2, [R3]       ; Almacenar el valor de R2 en la dirección de memoria apuntada por R3


Este programa mueve los valores 10 y 20 a los registros R0 y R1, respectivamente, los suma y guarda el resultado en R2. Luego, almacena el resultado en la dirección de memoria apuntada por R3.