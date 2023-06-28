# ✖️ Expresiones y declaraciones
Ya anteriormene hemos creamos valores y les aplicamos operadores a ellos para obtener nuevos valores. Crear valores de esta manera es la sustancia principal de cualquier programa en JavaScript. Pero esa sustancia tiene que enmarcarse en una estructura más grande para poder ser útil. Así que eso es lo que veremos a continuación.

Una **_expreción_** es un fragmento de código que produce algún valor. Cada valor que se escribe literalmente, como por ejemplo, 22 o "psicoanálisis", es una **_expreción_**. Una expresión[^1] entre paréntesis también es una expresión[^2], como lo es un operador binario aplicado a dos expresiones o un operador unario aplicado a una sola.

Esto demuestra parte de la belleza de una interfaz basada en un lenguaje. Las expresiones pueden contener otras expresiones de una manera muy similar a como las sub-oraciones en los lenguajes humanos están anidadas, una suboración puede contener sus propias sub-oraciones, y así sucesivamente. Esto nos permite construir expresiones que describen cálculos arbitrariamente complejos.

El tipo más simple de declaración es una expresión con un punto y coma después ella.
```javascript
const num = 1
let numEsUnNumero = true
!numEsUnNumero // false
```
Esto es un programa. Sin embargo, es un programa inútil. Una expresión puede estar feliz solo con producir un valor, que luego pueda ser utilizado por el código circundante. Una declaración es independiente por si misma, por lo que equivale a algo solo si afecta al mundo.

En algunos casos, JavaScript te permite omitir el punto y coma al final de una declaración. En otros casos, tiene que estar allí, o la próxima línea serán tratada como parte de la misma declaración. Las reglas para saber cuando se puede omitir con seguridad son algo complejas y propensas a errores.

Asi que cada declaración que necesite un punto y coma siempre tendra uno. Te recomiendo que hagas lo mismo, al menos hasta que hayas aprendido más sobre las sutilezas de los puntos y comas que puedan ser omitidos.


[^1]: En matemáticas, una expresión matemática es una combinación de símbolos que se pueden combinar con operaciones matemáticas como la suma, la resta, la multiplicación y la división. Los símbolos pueden representar números, variables, funciones, corchetes y puntuación. Una expresión matemática puede ser un objeto matemático o una fórmula que hace una afirmación sobre objetos matemáticos.

[^2]: En programación, una expresión es una combinación de constantes, variables o funciones, que es interpretada de acuerdo a las normas particulares de precedencia y asociación para un lenguaje de programación en particular. Como en matemáticas, la expresión es su valor evaluado, es decir, la expresión es una representación de ese valor
