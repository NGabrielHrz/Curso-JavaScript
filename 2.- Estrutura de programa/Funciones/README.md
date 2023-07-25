# 🖇️ Funciones

Una función es una pieza de programa envuelta en un valor. Dichos valores pueden ser *aplicados* para ejecutar el programa envuelto. Por ejemplo, en un entorno navegador, la vinculación prompt sostiene una función que muestra un pequeño cuadro de diálogo preguntando por entrada del usuario. Esta se usa así:

```javascript
prompt("Introducir contraseña");
```

Dando como resultado el siguiente cuadro de dialgo:

![promp]()

Y tal y como se explico antes, estas funciones ya vienen con el entorno, por lo que solo es necesario llamarlas. Ejecutar una función tambien se conoce como *invocarla*, *llamarla*, o *aplicarla*.

Un ejemplo de *llamar* a la fución es el siguiente:

```javascript
function HelloYou(yourName) {
  alert("Hello "+yourName);
}

HelloYou(prompt("Introducir nombre"))
```
Donde `prompt()` abre un cuadro dialogo donde puedes introducir algun argumento para la función, y esta devulve el valor introducido con un `alert()` saludandote.

## ➕ Un pequeño PLUS-ULTRA
Previamente habiamos trabajado con el siguiente ejemplo para calcular el area de un circulo usando la consola del navegador
```javascript
const PI = 3.1415926;

function AreaCirculo(r) {
  console.log(PI * Math.pow(r, 2));
}

AreaCirculo(5);
```
Pero ahora yo te reto a que realices los cambios necesarios para que puedas ingresar los datos con `prompt()` y que el resultado tambien sea un cuadro de dialogo del navegador. Diviertete con el😁.
