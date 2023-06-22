# ❓ Valores booleanos
Un valor booleano es una variable que puede tomar dos valores: `verdadero` o `falso`. En programación, los valores booleanos se utilizan para representar __condiciones lógicas__. Por ejemplo, si se desea saber si un número es mayor que otro, se puede utilizar una expresión booleana para representar la condición “el número es mayor que el otro”. El resultado de la expresión será verdadero o falso.

Aquí hay algunos ejemplos de valores booleanos:
```JavaScript
let esMayor = (5 > 3); // esMayor será true
let esMenor = (5 < 3); // esMenor será false
```
La primera condición es verdadera porque 5 es mayor que 3, y la segunda es falsa por que 5 no es menor que 3.

Si queremos saber si dos números son iguales, podemos usar otra condición lógica como esta:
```JavaScript
let esIgual = (4 === 4); // esIgual será true
let esIgual = (5 === 10); // esIgual será false
```
Esta condición es verdadera porque 4 es igual a 4, y 5 no es igual a 10.

## 😵‍💫 Formas de funcionalidad de las condiciones lógicas?
Las condiciones lógicas se pueden combinar con operadores lógicos como `AND`, `OR` y `NOT` para crear condiciones más complejas.

Por ejemplo, si queremos saber si un número es par **y** mayor que 10, podemos usar una condición lógica como esta:
```JavaScript
let n = 2; // 4, 6, 8

if (n % 2 === 0 && n < 10) {
  console.log(n + " es un número par y menor que 10");
}
else {
  console.log(n + " no cumple la condición");
}
```
Esta condición es verdadera solo si n es par y mayor que 10.

Si queremos saber si un número es par **o** mayor que 10, podemos usar una condición lógica como esta:
```JavaScript
let n = 2; // 4, 6, 8

if (n % 2 === 0 || n < 10) {
  console.log(n + " es un número par o menor que 10");
}
else {
  console.log(n + " no cumple la condición");
}
```
Esta condición es verdadera solo si n es par y mayor que 10.

Por otro lado, la condición `NOT` es diferente, cambia el *estado logico* de la condición, por ejemplo:
```JavaScript
(2 === "hola") // false
!(2 === "hola") // true
```

Sabemos que un numero no es igual a una palabra por eso la primera comparación es falsa, pero con un `NOT` podemos cambiar el valor booleano.

Las condiciones lógicas se usan mucho en la programación para controlar el flujo de un programa o para tomar decisiones basadas en los datos.