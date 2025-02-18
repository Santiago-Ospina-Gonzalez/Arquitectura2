# Arquitectura2S
Santiago:
1. Introduccion:
La Ley de Benford, también conocida como la ley de los primeros dígitos, es un fenómeno estadístico que describe la frecuencia con la que los dígitos ocurren en diversas colecciones de datos. A pesar de su aparente simplicidad, esta ley desafía la intuición, ya que sostiene que en muchos conjuntos de datos del mundo real, los números que comienzan con el dígito 1 aparecen con más frecuencia que los números que comienzan con el 2, y estos a su vez son más frecuentes que los que comienzan con el 3, y así sucesivamente. 

Esta distribución de dígitos no es aleatoria, sino que sigue una proporción logarítmica: aproximadamente el 30% de los números en un conjunto de datos empiezan con el dígito 1, el 17.6% con el 2, el 12.5% con el 3, y así en descenso. La ley fue observada por primera vez por el matemático Frank Benford en 1938, aunque ya había sido descrita anteriormente por Simon Newcomb en 1881. 

La Ley de Benford ha encontrado aplicaciones en una variedad de campos, desde la contabilidad forense hasta la ciencia de datos debido a su capacidad para detectar irregularidades y fraudes, ya que los datos manipulados o falsificados tienden a mostrar una distribución de dígitos diferente a la esperada según esta ley.

Josefo: 
3. Ensamblador:

Ley de Benford y su Implementación en Ensamblador
Implementar la Ley de Benford en lenguaje ensamblador implica procesar una lista de números y contar la frecuencia de los primeros dígitos. Para ello, necesitamos:

Leer o almacenar datos numéricos en memoria.
Extraer el primer dígito de cada número.
Incrementar un contador para cada posible primer dígito (del 1 al 9).
Mostrar los resultados para analizar la distribución.

    - Instrucciones:

Instrucciones Claves en Ensamblador
En un programa en ensamblador, podríamos usar instrucciones como:

MOV: Para mover valores entre registros y memoria.
DIV: Para dividir números y extraer dígitos.
CMP y JUMP (JMP, JE, JNE, etc.): Para comparar y controlar el flujo del programa.
LOOP: Para recorrer los datos en un ciclo.
INT 21h (DOS) o SYSCALL (Linux): Para entrada/salida de datos.
