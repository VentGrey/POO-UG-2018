# Ciclos


## For

La segunda estructura de control es lo que conocemos como ciclos, el primero
que veeremos es quizá el mas popular de todos, llamado `for`:

Los tres componentes del ciclo for (separados por un semicolon `;`) son:

1. La declaración/inicialización de una variable

2. La condicional

3. La sentencia de incremento o decremento.

* La declaración de la variable se hace una sola vez, como si ésta fuese
colocada al incio de las llaves `{` en la primera iteración del código.

* Después la condición se revisa, si ésta retorna un `true` entonces el cuerpo del ciclo for se ejecutará, si retorna un `false` el ciclo se detendrá.
* Asumiendo que el ciclo continúa, el cuerpo del bloque de código se ejecutará y cuando finalmente se encuentre la llave de cierre `}` la sentencia de incremento se ejecutara antes de que la condición se revise de nuevo.


Ejemplo:
```java
for (int i = 0; i < 100; i++) {
    System.out.println(i + " elefante se columpiaba sobre la tela de una araña");
}
```

> Las llaves son opcionales (puedes crear ciclos en una sola línea)
> si el ciclo contiene solo una sentencia, pero siempre es recomendable
> utilizar llaves para evitar malentendidos y errores.

## While


