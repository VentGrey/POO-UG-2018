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
caracter en mayúsculas y que se encuentre en *"Nomeclatura camino"*
(En la cual la primera letra de cada palabra debera ser una mayúscula).


