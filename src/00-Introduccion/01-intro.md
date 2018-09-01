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

En la programación Orientada a Objetos, encontraremos algunos conceptos cotidianos
, la importancia de familiarizarse con ellos facilitara la interpretación de ésta
metodología de programación.

Las siguientes definiciones son tomadas de la *Real Academia Española* y del
diccionario *Larousse*, posteriormente se expondrá un concepto más concreto
y práctico, acompañado de algunos ejemplos.

**Paradigma**: " *Teoría o conjunto de teorías cuyo núcleo central se acepta sin cuestionar y que suministra base y modelo para resolver problemas y avanzar en el conocimiento* ".

De manera concreta podemos definir:
**Paradigma es el modo o la forma natural de hacer algo**. Lo podemos ver
normalmente utilizado en "Paradigma de la Programación Orientada a Objetos"

**Abstracción**: " *Separar por medio de una operación intelectual un rasgo o una cualidad de algo para analizarlo aisladamente o considerarlo en su pura esencia o noción* ".

## Veamos un ejemplo

Lo primero que se nos podría venir a la mente con la palabra "Planta" es un
ser vivo, con hojas color verde, que posee un tallo y raíces, sin embargo, en
este enfoque existe una gran diversidad de plantas. Ahora, si le pedimos imaginar
la palabra "Planta" a un electricista o a un empleado que trabaja como técnico
en el proceso de purificación del agua, posiblemente ambos imaginarán cosas
totalmente diferentes, el primero podría imaginar la localización donde toda
la maquinaria y el cableado se encuentra para abastecer de luz eléctrica a
una región, el otro podría imaginar su central de agua donde ésta es purificada.

Si le preguntamos a un niño o a un adulto que nos describa la palabra "Nube" y
ellos no estén familiarizados con la tecnología, nos podrían decir que es
el agua en su tercer estado de la materia (gas) y que se encuentra en el cielo.

Sin embargo, si le preguntamos a una persona muy familiarizada con la tecnología
 y el internet de las cosas entonces podría contestarnos que "Nube" es aquel
 data center donde se almacenan y respaldan datos de diversos usuarios.

> Otros mas extremos podrían decirnos que "Nube" es el método de transporte
> volador de un personaje muy famoso.

Si una persona que vive en la ciudad cierra los ojos por uno o dos minutos y
piensa en un vehículo, lo primero que podria imaginar seria un medio de
transporte con cuatro ruedas, un motor y un armazón probablemente de color
rojo. Sin embargo, si preguntamos lo mismo a alguien que vive en una zona
costera o muy cercana a la playa y que esté relacionada con actividades
pesqueras podrían imaginar un barco o un bote ya que también son vehículos
submarinos. Si abrimos mas los paronarmas tenemos los aviones, helicópteros,
naves y cohetes espaciales, todos estos son vehículos, cada uno con sus
diferentes características( **Atributos** ) y funciones ( **Métodos** ).

## ¿Modularidad?

El sistema de producción modular, ha tenido su origen desde hace muchos años
atrás, vino a revolucionar la forma de producción, abaratando sus costos
y facilitanto a la industria, el proceso de la producción en masa, por
ejemplo, antes era muy costoso fabricar una pistola artesanal, sin embargo,
cuando alguien decidió modular el objeto en varias partes y enfocarse
exclusivamente en la fabricación y producción de los módulos para
posteriormente ensamblarlos, obtuvieron excelentes resultados en tiempo,
calidad del producto y costos de inversión. Ademas, dio origen a la producción
de estándares, permitiendo el reemplazo de ciertos módulos para el proceso de
mantenimiento y mejoras.

Retomando el tema del revólver artesanal, intentemos tomar el enfoque de la
programación, inicialmente el proceso de producción del software era de
manera estructurada, es decir era muy costoso, eso sin considerar el proceso
de mantenimiento. Imagina revisar un archivo con 135,000 líneas de código,
buscar errores, corregirlos, mantener actualizado el software, no era una
tarea fácil ni óptima, demás, sería muy difícil que alguien intentara
reutilizar el código, pues el software está hecho para satisfacer las
necesidades específicas de un cliente.

Por lo tanto, la modularidad en la programación nos otorga múltiples ventajas
como:
 * Simplificación de un problema complejo en varios subproblemas más simples
 * Reutilización de código
 * Facilidad en el proceso de mantenimiento y producción.
 * Reducción de líneas de código.
 * Facilidad en la legibilidad y compresión del código.

Con ello podemos ver una ligera introducción a lo que haremos dentro de
éste libro, aprenderemos a programar orientado a objetos, así que manos a la obra.
