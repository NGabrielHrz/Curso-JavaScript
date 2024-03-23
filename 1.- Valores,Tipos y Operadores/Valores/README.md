# 👾 Valores
Anteriormente ya habiamos visto que al hablar de las computadoras, tambien hablamos de los `datos` y que estos en si, solo son un monton de *`bits`*.

Ahora veremos lo que son los valores, para ello, hay que tener en cuenta que las computadoras modernas tienen mas de 30 billones de bits en su almacenamiento de datos volatil (**`RAM`**) y los discos duros, que suelen tener muchisima mas capacidad.

## 👷 Trabajar con valores.
Para que podamos trabajar con una gran cantidad de *`bits`* sin perdernos nesicitamos separarlos en **bloques** que representen ***Pedazos*** de infromación. Y en ![JavaScript Logo](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=white), estos **bloques** los llamamos ***`Valores`***. Cada valor que determian su "**rol**", estos roles pueden ser:

| Tipos de valores | Descripción |
|--------------|-------------|
| Números      | Representan valores numéricos (enteros o de punto flotante). |
| Cadenas de texto   | Representan una secuencia de caracteres. |
| Booleanos    | Representan valores de verdad (`true` o `false`). |
| Arreglos     | Estructuras para almacenar múltiples valores en una variable. |
| Objetos      | Estructuras de datos con propiedades y métodos. |
| Null         | Representa la ausencia intencional de valor. |
| Undefined    | Representa una variable declarada pero sin valor asignado. |
| Funciones    | Pueden asignarse a variables, pasarse como argumentos y devolverse como valores de otras funciones. |
> Cabe recalcar que estos tipos de valores son generales y no son todos los que puede llegar a tener JavaScript.

Para poder crear un *valor* solo debemos invocar su nombre, y como se puede apreciar en la tabla, hay de diferentes tipos, un ejmplo que podemos utilizar es uno ya visto anteriormente:
```Javascript
let yourName ="Pon tu nombre aquí"; // Aqui donde la palabra reservada "let" se usa para identificar una variable
function HelloYou() { // Aqui donde la palabra reservada "function" se usa para indicar el comienzo de una función
  console.log("Hello "+yourName); // La palabra "console" para que la consola sea llamada y "log" para escribir en la consola
}

HelloYou()
```
>Recuerda que de este ejemplo cuedes cambiar algunos parametros para probar diferentes mensajes.
