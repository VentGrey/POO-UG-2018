# El lenguaje de programación Java

Java es un lenguaje de programación con mas de 20 años en existencia
y siendo uno de los lenguajes de programación mas populares actualmente,
usado para cosas tan cotidianas como tu teléfono inteligente hasta
sondas que vigilan otros planetas (Si, curiosity utiliza Java en su
programación).

## Un poco de historia de Java

Java es un lenguaje de programación creado por una compañía de nombre
*Sun Microsystems* en los años 80 que básicamente dominaba el mercado
con sus workstations de alta potencia en aquellos tiempos, aunque a
principios de los años 90, Sun Microsystems comenzó a enfocarse mas en
vender servidores debido a que en esos años la web estaba naciendo.

Durante el desarrollo de la compañía un pequeño grupo de desarrolladores
llamado "The Green Project" buscaban hacer una alternativa sencilla a
C++, en el proceso de crecimiento crearon un proyecto al cual llamaron
Oak y fue durante el crecimiento de Oak donde la Web comenzó a poblarse,
al ver que la web evolucionaba soportanto texto con formato, hasta
imágenes y video, entonces ¿por qué no agregar contenido interactivo?
Oak ya tenía la mayor parte del problema resuelto. Normalmente el
internet está lleno de computadoras de todo tipo de arquitecturas,
sistemas operativos e incluso navegadores web sería una tarea laboriosa
y desgastante que cada programa tuviese que ser escrito para soportar
todos y cada uno de ellos, con Oak el panorama cambiaba pues las personas
solo necesitaban incluir una versión de un solo programa y si usabas
un navegador web que soportara a Oak podías ejecutar el programa.

En 1994 el equipo se dedicó a desarrollar su propio navegador web llamado
"WebRunner" aunque para ese tiempo el lenguaje no se llamaba "Oak", después
de ver que el nombre estaba registrado por una marca de microcontroladores
y de mucho pensamiento en el nombre, los integrantes decidieron llamar al
proyecto "Java".

> Una curiosidad es que Chris Warth propuso el nombre al verlo en su bolsa de
> café que leía "Mocca-Java" después de una sesión de hacking intensa.

El navegador WebRunner pronto migró a un nombre nuevo llamado "HotJava" para
que encajara un poco mas con el nombre del lenguaje en cuestión.

En 1995 se invito a los desarrolladores de Java a la TED 6 para que presentaran
Java a un grupo de profesionales de la web, al inicio hubo pánico porque el
programa se caía en sus primeras versiones, pero afortunadamente ese no fue el
caso en la conferencia. Al inicio la gente no presentaba ningún interes en el
clon de un navegador existente ("Mosaic"), pero en el momento en el que algo
se movió en la pantalla se captó la atención total del público y en Marzo de
1995 Java liberó su primera versión al público, empezando por números de 2 cífras
y terminando con números de 4 cifras al final del mes.

Desde ese día la JVM se ha portado a miles de dispositivos, desde una TV en casa
hasta las 2 sondas exploradoras de marte envíadas en 2004.

Irónicamente Java es usado en muchos tipos de sistemas computacionales y fué
olvidado en la web, lo que le dió tanta popularidad en un principio.

# Conceptos básicos de la programación orientada a objetos

Programación orientada a objetos ¿qué es?. Nos pofremos encontrar con algunos
conceptos que son utilizados de manera cotidiana, es importante poder
familiarizarse con estos conceptos para poder interpretar con mayor facilidad
esta nueva "metodología" de programación. Primero facilitaremos el significado
mas representatifo que proporciona la RAE ( *Real Academia Española* )
y al final se expondrá un concepto más concreto y práctico.

**Paradigma**: *"Teoría o conjunto de teorías cuyo núcleo central se acepta sin
cuestionar y que se suministra la base y modelo para resolver problemas y
avanzar en el conocimiento"*

Fuente:(RAE: *http://dle.rae.es/?id=RpXSRZJ*)

De manera que podemos definir:
*Paradigma es el modo o la forma de hacer algo*. Lo podremos ver normalmente
utilizado en el paradigma de programación orientado a objetos.

Concretizando:
**Abstracción es lo percibido de una realidad en determinado contexto**.
Tomemos como ejemplo las siguientes palabras y posteriormente explicaremos los
contextos:
 * Planta
 * Nube
 * Vehículo
 * Ratón
 * Llave

Lo primero que podria llegar a nuestra mente con la primera palabra (Planta) es
un ser vivo con hojas color verde, que posee un tallo y raíces, sin embargo,
existen diferentes tipos de plantas en este enfoque. Pero ¿qué sucede si le
preguntamos a un electricista? ¿A un trabajador en el área técnica de proceso
de purificación del agua? Posiblemente estén pensando que "Planta" se refiere a
las instalaciones donde tienen la maquinaria para generar energía o para
purificar el agua (respectivamente).
