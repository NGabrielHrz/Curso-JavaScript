# 📝 Strings
Un string es una secuencia de caracteres que representa un texto. En JavaScript, los strings se pueden crear usando comillas simples (''), comillas dobles ("") o comillas invertidas (``), este ultimo casi no se usa, pero es util saberlo. Los strings tienen una propiedad llamada length que indica el número de caracteres que contienen. También tienen varios métodos que permiten manipularlos, como concatenarlos, dividirlos, reemplazarlos, convertirlos a mayúsculas o minúsculas, etc.

Por ejemplo, el siguiente código crea un string con el texto "Hola mundo" y lo asigna a la variable saludo:
```JavaScript
let saludo = "Hola mundo";
console.log(saludo);
```
Para acceder a un caracter específico de un string, se puede usar la notación de corchetes ([]), indicando el índice del caracter deseado. Los índices empiezan en 0, por lo que el primer caracter tiene el índice 0, el segundo el índice 1, y así sucesivamente, justo como se muestra en la tabla:
| H | o | l | a | space | m | u | n | d | o |
| --- | --- | --- | --- | :---: | --- | --- | --- | --- | --- |
| 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 |

El siguiente código muestra el primer y el último caracter del string saludo:
```JavaScript
console.log(saludo[0]); // H, ya que es el primer caracter como se muentra en la tabla
console.log(saludo[saludo.length - 1]); // o
```
> Se usa .length para saber la longitud de la palabra, pero .length empieza a contar desde "1" por eso se le resta 1, ya que si no se realiza la resta, el resultado es 10, y como se muestra en la tabla, no existe un caracter en la 10ma posición, por lo que macaria error.

Para concatenar dos o más strings, se puede usar el operador (+), que devuelve un nuevo string con la unión de los strings originales. Por ejemplo, el siguiente código crea un nuevo string con el texto "Hola mundo, soy Bing" y lo asigna a la variable mensaje:
```JavaScript
let mensaje = saludo + ", soy Tyrone";
console.log(mensaje);
```
Para dividir un string en varios sub-strings según un separador, se puede usar el método split(), que devuelve un array con los sub-strings resultantes. Por ejemplo, el siguiente código divide el string mensaje por los espacios y guarda el array en la variable palabras:
```JavaScript
let palabras = mensaje.split(" "); // ["Hola", "mundo,", "soy", "Tyrone"], muy util para manipular datos
console.log(palabras);
```
Para reemplazar una parte de un string por otra, se puede usar el método replace(), que devuelve un nuevo string con la sustitución realizada. Por ejemplo, el siguiente código reemplaza la palabra "Bing" por "Google" en el string mensaje y guarda el resultado en la variable otroMensaje:
```JavaScript
let otroMensaje = mensaje.replace("Tyrone", "Pablo"); // "Hola mundo, soy Pablo"
console.log(otroMensaje);
```
Para convertir un string a mayúsculas o minúsculas, se pueden usar los métodos toUpperCase() y toLowerCase(), que devuelven nuevos strings con la conversión aplicada. Por ejemplo, el siguiente código convierte el string saludo a mayúsculas y lo guarda en la variable saludoMayus:
```JavaScript
let saludoMayus = saludo.toUpperCase(); // "HOLA MUNDO"
let saludoMinus = saludo.toLowerCase(); // "hola mundo"
console.log(saludoMayus);
console.log(saludoMinus);
```
