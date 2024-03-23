# Valores  de retorno
El hecho de mostrar un cuadro de dialogo o escribir texto en la pantalla es lo que se conoce con un _efecto secundrario_ del metodo _**console.log**_. Muchas funciones son utiles debido a los efectos secundarios que ellas producen.

Existen metodos que pueden producir valores, que en cuyo caso, no es necesario que tenga efectos secundarios, un ejemplo de estos metodos es `Math.max()`.

### Ejemplo

```javascript
console.log(Math.max(2,4));
// -> 4
```
En este caso, lo que hace el metodo `Math.max()` busca el número mas grande, el cual es 4 en el ejemplo.

> [!TIP]
> Esto se puede probar de con diferentes números para, y en caso contrario existe `Math.min()`, el cual regresa el número mas pequeño.

Cundo un metodo produce un valir se dice que _retorno_ dicho valor. Todo lo que produce un valor es una expresión en Javascript, esto significa que las llamadas a los metodos se pueden usar dentro de expresiones mas grandes.

```javascript
console.log(Math.min(2, 4) + 100);
// → 102
```
> [!INFO]
> Lo que sucede en el codigo anterior es simple logica aritmetica, en `(2, 4) + 100` se le suma 100 a cada uno de los numeros dentro de la de los parentesis, lo cual quedaria (102, 104) en este caso, lo unico que hace `Math.min()` es buscar el mas pequeño de los dos.

