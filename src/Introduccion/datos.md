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

## El tipo caracter

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


