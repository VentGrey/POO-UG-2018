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


