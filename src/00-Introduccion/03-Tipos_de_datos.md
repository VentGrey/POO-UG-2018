# Tipos de dato en Java

En Java existen diferentes tipos de datos los cuales pueden ser primitivos o
propios del lenguaje.

Java posee 8 tipos de dato primitivos: `byte`, `short`, `int`, `long`, `char`
`boolean`, `float` y `double`.


## La tabla de los tipos

Es mejor ejemplificar que solo decir, aquí hay una tabla con todos los rangos de
valores que los tipos primitivos pueden tomar en Java.

| Tipo | Representación numérica | Rango de valores | Valor por defecto |
|------|-------------------------|------------------|-------------------|
|booleano| No tiene | `true` & `false` | `false` |
| byte | 8 bits con signo | \\(-27 \\) hasta \\(27 - 1\\) | 0 |
| short | 16 bits con signo |\\(-128 \\) hasta \\( +27 \\) & \\(-32,768 \\) hasta \\(+32,767\\)  | 0 |
| int | 32 bits con signo |\\(-231 \\) hasta \\(231 - 1\\) & \\(-2,147,483,648 \\) hasta \\(+2,147,483,647\\) | 0 |
| long | 64 bits con signo |\\(-263 \\) hasta \\(263 - 1\\) & \\(-9,223,372,036,854,775,808 \\) hasta \\(9,2223,372,036,854,775,807\\))| 0L |
| float | punto flotante de 32 bits |\\(1.401298464e-45 \\) hasta\\(3.402823466e+38 \\) (positivo o negativo) | 0.0F|
| double | punto flotante de 64 bits |\\(4.940656458411246544e-324d\\) hasta \\(1.79769313486231570e+308d\\) (positivo o negativo) | 0.0D |
| char | 16 bits sin signo |\\(0\\) hasta \\(216-1\\) & \\(0 \\) hasta \\(65,535\\)| 0 |

> Notas:
> Java 8  y posterior provee métodos para realizar operaciones aritméticas sin signo en `int` y `long`.
> Un carácter convencionalmente representa una unidad Unicode/UTF-16
> Aunque el booleano contiene solo un bit de información, su tamaño en la memoria varia dependiendo de la JVM.


## El tipo carácter

El tipo `char` nos permite guardar un único carácter Unicode de 16 bits en memoria
. Dicho carácter debera ser rodeado por comillas simples.

```java
char caracter1 = 'a';
char caracter2 = '4';
char caracter3 = 65; // caracter3 == A
```

Asimismo podemos utilizar otras secuencias de escape:

```java
char tab = '\t';
char backspace = '\b';
char newline = '\n';
char Carriagereturn = '\r';
char formfeed = '\f';
char singlequote = '\'';
char doublequote = '\"';
char backslash = '\\';
char unicode = '\uXXXX' // Siendo XXXX el valor del caracter unicode que quieras representar.
```

## El tipo float

Un flotante (`float`) es un número de punto flotante de 32 bits de presición
simple.

En Java los decimales se tratan como `double` por defecto.
Para crear un `float`, simplemente se le agrega una `f` al decimal literal.

```java
double ejemplodoble = 0.5; //Sin  f después de los dígitos == double
float ejemplofloat = 0.5f; //Con f después de los dígitos == float

float pedro = 92.7f; //El es pedro el flotante...
float pedro_positivo = 89.2f; //Puede ser positivo :)
float pedro_negativo = 45.5f; //O negativo :(
float pedro_entero = 23.0f; //Puede ser un número entero (no un int)
float pedro_diminuto = 0.243; //Puede ser un valor fraccionario menor a 0
```
> Los flotantes pueden manejar 5 operaciones aritméticas comunes:
> Suma (+)
> Resta (-)
> Multiplicación (*)
> División (/)

## El tipo entero

No podemos hablar de puntos flotantes sin ver el tipo primitivo llamado `int` el
cual es un tipo de dato primitivo que retiene valores de números completos, es
decir, números que no poseen un aditamento decimal o fraccionario.

Citando al API de Java:
> "La clase Integer envuelve a un calor del tipo primitivo int en un objeto. Un
> objeto de tipo Integer contiene un solo campo cuyo tipo es `int`.

Los enteros por defecto ocupan 32 bits y son con signo, pueden guardar valores
desde el mínimo \\(-231\\) hasta un valor máximo de \\(231-1\\).

```java
int ejemplo = -42; //El significado de la vida, el universo y todo para los negativos.
int otroejemplo = 248;
int entero = 73;

int suma_de_enteros = otroejemplo + entero;
int resta_de_enteros = ejemplo - entero;
```

## El tipo doble

Un `double` es un tipo de dato de punto flotante con doble precisión.

```java
double ejemplo = -7421.34; //Puede ser negativo
double otroejemplo = 2093.59; //O positivo
```
Como curiosidad, por la manera en la que los números de punto flotante se
guardan muchos de éstos no poseen una representación exacta:

```java
double noexacto = 1.32 - 0.42; //El resultado debería ser 0.9
System.out.println(noexacto); //0.90000000000000001
```

Si queremos usar un tipo de dato para guardar valores de precisión aceptable
un `double` es nuestra mejor opción, aunque no se recomienda si queremos
valores con precisión alta, para ello necesitamos la clase `BigDecimal`.

## El tipo long

El tipo `long` es un entero de 64 bits con signo. (Desde Java 8 el tipo puede
ser usado con signo o sin signo).

```java
long ejemplo = -42;
long ejemplo2 = 285;
```

> Al igual que los flotantes, podemos agregar una "L" después del número
> para convertirlo a un `long`.

```java
long numeroenorme = 549755813888L;
```

> Además, la "L" que se agrega al final de la cifra no es sensible a mayúsculas
> o minúsculas, por lo que usar "l" también es válido.
