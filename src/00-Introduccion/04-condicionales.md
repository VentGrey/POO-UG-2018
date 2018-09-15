# Condicionales

La sentencia `if` es la sentencia mas básica que existe dentro del control
de flujo en Java, ésta le indica al programa que debería ejecutar cierto bloque
de código *solo y solo si* una evaluación en particular devuelve como resultado
un booleano con valor `true`.

Veamos el ejemplo con una bicicleta, todos hemos tenido una y sabemos que entre
mayor es nuestra velocidad mas probable es que suframos un accidente, un
código en Java que represente nuestro juicio en esa situación podría ser:

```java

void UsarFrenos() {
    // para el if la bicicleta debe de estar en movimiento
    if (SeMueve) {
        VelocidadActual -- ;
    }
}
```

Un ejemplo un poco mas acercado a los números podría ser:

```java

if (i < 2) {
    System.out.println("i es menor que 2");
} else if (i > 2) {
    System.out.println("i es mayor que 2");
} else {
    System.out.println("i no es menor que 2 ni mayor que 2");
}
```

Aquí podemos ver una sentencia nueva llamada `else` el cual es un "camino"
secundario en caso de que la evaluación de la sentencia `if` retorne un `false`,
si lo acomplamos al ejemplo de la bicicleta que escribimos en la parte
superior podemos verlo de ésta forma:

```java
void UsarFrenos() {
    if (SeMueve) {
        VelocidadActual --;
    } else {
        System.err.println("La bicicleta no se esta moviendo ._. ");
    }
}
```

