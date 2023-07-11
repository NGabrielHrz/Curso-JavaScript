# 🔗 Vinculaciones
Hasta ahora hemos visto cómo producir nuevos valores a partir de valores anteriores, pero esto no cambia los valores anteriores, y el nuevo valor tiene que ser usado inmediatamente o se disipará nuevamente. Para atrapar y mantener valores, JavaScript proporciona una cosa llamada vinculación, o variable:
```javascript
let atrapado = 5 * 5;
```
En este ejemplo la palabra reservada `let` es usada para indicar que se hara una vinculación. El siguiente es el nombre de la vinculación, y si queremos darle un valir de inmediato, un operador `=` seguido de una expresión.

La declareación anterior crea una vinculación de nombre *"atrapado"* y captura el numero resultante de la expresión.

Una vez definida la vinculación su nombre puede ser usado para para otra expresión, por ejemplo:
```javascript
let ten = 10;

console.log(ten * 10); // -> 100
```

## Asignación de la vinculación
Hay que mencionar que el hecho de que a la vinculación se le asigne un valor de forma inmediata, este puede cambiar haciendo uso de el operador `=` en cualquier momento.
```javascript
let tipoChiste = ligero;
console.log(tipoChiste); // -> ligera

tiporChiste = negro;
console.log(tipoChiste); // -> negro
```

Una forma de ver las vinculaciones son como como un gancho, ya que estas no *continen* valores, si no que estas agarran los valores. Ademas, un programa solo puede acceder a los valores que todavia pueda referenciar, por ejemplo:
```javascript
let miNombre = 'Shouko';
console.log(miNombre); // -> Shouko

miNombre = miNombre + ' Komi'
console.log(miNombre); // -> Shouko Komi
```

Cabe recalcar que cuando no se le asigna ningun valor a la vinculación esta queda *vacía* por lo que el gancho, o Hook en ingles, no tendar nada que agarrar y terminara mostrando un `undefined`.