# Estructura básica de un programa

## El lenguaje usado en la materia será JAVA (v8+)

Java es un lenguaje de programación orientado a objetos,
desarrollado por Sun Microsystems (Oracle hoy) a principios
de los años 90. El lenguaje en si mismo toma mucha de su sintáxis de C & C++,
pero tiene un modelo de objetos mas simple y elimina las herramientas de bajo
nivel, que suelen inducir a muchos errores como la manipulación directa de
punteros o memoria.

### Estructura básica de un programa de Java

```java
public class HolaMundo {
    public static void main(String[] args){
        System.out.println("Hola Mundo!");
    }
}
```

Analicemos éste código mas detenidamente:

1. La clase `HolaMundo` es pública esto quiere decir que podemos ejecutarla
desde la línea de comandos o terminal.

2. Todos los argumentos de Java deberán ser agrupados con llaves `{}`, siendo
la llave abierta el inicio del grupo de argumentos `{` y la llave cerrada el
fin de éste mismo `}`.

> Nota: Para que Java reconozca ésto como una clase pública (y que no esté
> escupiendo errores en consola), el nombre del archivo deberá ser el mismo que
> el de la clase en cuestión (HolaMundo en este caso) con la extensión .java

Las convenciones de nombres recomiendan que las clases de Java comienzen con un
caracter en mayúsculas y que se encuentre en *"Nomeclatura camello"*
(En la cual la primera letra de cada palabra debera ser una mayúscula).

## Proceso de compilación

El compilador, una vez procesa el archivo `.java` éste generará un archivo del
tipo `bytecode` y éste al final es interpretado por la JVM (Java Virtual Machine).

De manera opcional el compilador también puede procesar anotaciones encontradas
en archivos fuente y `.class` usando la anotación `Pluggable`.


## Descomponiendo a "HolaMundo"

El primer HolaMundo que creamos contiene un único archivo que consiste de una
definición de clase llamada `HolaMundo`, un método `main` y una sentencia dentro
del método `main`.

```java
public class HolaMundo {
```

La palabra clave `class` comienza la definición de una clase, llamada `HolaMundo`.
Toda aplicación de Java contiene al menos una definición de clase.

```java
public static void main(String[] args) {
```

El método `main` es un punto de entrada para todo programa en Java, por lo que
siempre debe de existir uno, sus componentes son:

`public`: Significa que el método puede ser llamado desde cualquier parte dígase
fuera del mismo programa.

`static`: Significa que existe y puede ser ejecutado por si mismo (a nivel clase)
`void`: Significa que el método retorna *nada*.

> Java, a diferencia de C y C++ no tiene un entero como un código de retorno
> la manera de Java es usando `System.exit()`

Dentro del método main podemos ver algo llamado "parametros":

```java
public static void main(String[] args)
```
------------------------------------------------------------------------------
Un arreglo de cadenas de nombre `args` como argumentos a la función principal.

> Nota: `args` es el nombre de una variable, así que puedes renombrarle.
------------------------------------------------------------------------------


Dentro del método `main` podemos ver la siguiente sentencia:

```java
System.out.println("Hola Mundo!");
```
Si rompemos la sentencia elemento por elemento:

| Elemento | Propósito |
|----------|-----------|
| `System` | Denota que la sentencia siguiente llamará a la clase `System` del paquete `java.lang`. |
| `.` | Es un operador `punto`. Éstos operadores proveen acceso a los miembros de las clases, en éste caso, sus variables o sus métodos, el operador punto de este caso nos dejara acceder al campo dentro de la clase `System`. |
| `out` | Es el nombre del campo estático del tipo `PrintStream` dentro de la clase `System` que contiene la funcionalidad de salida estandar. |
| `.` | Otro operador punto :P |
| `println` | Éste es el nombre del método dentro de la clase `PrintStream`. Éste método en particular imprime los contenidos de los parametros hacia la consola e inserta una nueva línea al finalizar. |
| `(` | Un paréntesis que indica que se está accesando a un método e indica el comienzo de los parámetros para el método `println` que estaremos usando |
| `"Hola Mundo!"` | Es una cadena que se pasa como parámetro al método `println` las comillas dobles indican el inicio y el fin de la cadena usada. |
| `)` | Otro paréntesis :B |
| `;` | Un punto y coma o *"semicolon"* el cual marca el fin de una sentencia. |

> ES IMPORTANTE NO OLVIDAR EL PUNTO Y COMA AL FINAL DE UNA INSTRUCCIÓN

