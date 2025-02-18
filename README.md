# Arquitectura2S
Santiago:
1. Introduccion:
La Ley de Benford, también conocida como la ley de los primeros dígitos, es un fenómeno estadístico que describe la frecuencia con la que los dígitos ocurren en diversas colecciones de datos. A pesar de su aparente simplicidad, esta ley desafía la intuición, ya que sostiene que en muchos conjuntos de datos del mundo real, los números que comienzan con el dígito 1 aparecen con más frecuencia que los números que comienzan con el 2, y estos a su vez son más frecuentes que los que comienzan con el 3, y así sucesivamente. 

Esta distribución de dígitos no es aleatoria, sino que sigue una proporción logarítmica: aproximadamente el 30% de los números en un conjunto de datos empiezan con el dígito 1, el 17.6% con el 2, el 12.5% con el 3, y así en descenso. La ley fue observada por primera vez por el matemático Frank Benford en 1938, aunque ya había sido descrita anteriormente por Simon Newcomb en 1881. 

La Ley de Benford ha encontrado aplicaciones en una variedad de campos, desde la contabilidad forense hasta la ciencia de datos debido a su capacidad para detectar irregularidades y fraudes, ya que los datos manipulados o falsificados tienden a mostrar una distribución de dígitos diferente a la esperada según esta ley.

Josefo: 3. Ensamblador:

Ley de Benford y su Implementación en Ensamblador Implementar la Ley de Benford en lenguaje ensamblador implica procesar una lista de números y contar la frecuencia de los primeros dígitos. Para ello, necesitamos:

Leer o almacenar datos numéricos en memoria. Extraer el primer dígito de cada número. Incrementar un contador para cada posible primer dígito (del 1 al 9). Mostrar los resultados para analizar la distribución.

- Instrucciones:
Instrucciones Claves en Ensamblador En un programa en ensamblador, podríamos usar instrucciones como:

MOV: Para mover valores entre registros y memoria. DIV: Para dividir números y extraer dígitos. CMP y JUMP (JMP, JE, JNE, etc.): Para comparar y controlar el flujo del programa. LOOP: Para recorrer los datos en un ciclo. INT 21h (DOS) o SYSCALL (Linux): Para entrada/salida de datos.

Alejandro: Flujo de trabajo:

El flujo de trabajo de nuestro equipo se basa en la metodologí Scrum, marco de gestión de proyectos que facilita la estructura y prácticas de trabajo, además a cada miembro del equipo se le asignará un rol especifico.

Las herraminetas que utilizaremos para realizar el proyecto integrador son las siguientes:

Frontend:

● Angular: Framework utilizado para el desarrollo del frontend de la plataforma web,
permitiendo la creación de interfaces dinámicas y funcionales.
● Node.js: Utilizado como entorno de ejecución para desarrollar herramientas
relacionadas con el frontend.
● Bootstrap: Framework de CSS utilizado para facilitar el diseño responsivo y la
creación rápida de componentes estilizados en el frontend.
● Figma: Herramienta utilizada para la creación de prototipos y diseño visual del
frontend.

Backend:

● Java Spring Boot: Framework para la construcción del backend, facilitando la
creación de APIs REST y la lógica del negocio.
● PostgreSQL: Base de datos relacional utilizada para la gestión y almacenamiento
de datos.

Infraestructura:

● AWS: Plataforma en la nube empleada para alojar y desplegar la aplicación y sus
componentes.
● Docker: Herramienta para contenerizar aplicaciones, facilitando el despliegue y la
portabilidad.
● Bitvise: Software utilizado para conectar y gestionar servidores Linux durante los
procesos de despliegue.

Gestión del Proyecto:

● Jira: Plataforma para la planificación y seguimiento de tareas, con un enfoque en la
metodología Scrum.
● Slack: Herramienta de comunicación y colaboración utilizada por el equipo.
● Jitsi: Solución de videoconferencia para reuniones y coordinación entre los
miembros del equipo.

● Metodología Scrum: Marco ágil utilizado para la organización y desarrollo iterativo
del proyecto.

Control de Versiones:

● GitHub: Plataforma de control de versiones utilizada para almacenar, gestionar y
colaborar en el código fuente del proyecto.

Angel Cuero

como hacer un hola mundo en assembly para ARM:

.globl _start
_start:
ldr r0,=0x101f1000
@ ASCII codes stored
@ at [r0] get printed
mov r1, #104 @ 'h'
str r1,[r0]
mov r1, #101 @ 'e'
str r1,[r0]
mov r1, #108 @ 'l'
str r1,[r0]
mov r1, #108 @ 'l'
str r1,[r0]
mov r1, #111 @ 'o'
str r1,[r0]
mov r1, #32 @ ' '
str r1,[r0]
mov r1, #119 @ 'w'
str r1,[r0]
mov r1, #111 @ 'o'
str r1,[r0]
mov r1, #114 @ 'r'
str r1,[r0]
mov r1, #108 @ 'l'
str r1,[r0]
mov r1, #100 @ 'd'
str r1,[r0]
my_exit: @do infinite loop at the end
b my_exit
