# 🫥 Valores vacios
Ya antes se habia visto un valor vacio, el cual es `undefined` (*indefinido*), se usa cuando no definimos el tipo de dato de una variable, constante o cuando se crea una función, justo como el siguiente ejemplo:
```javascript
let operacion // --> undefined
let num1 = 0 // --> number
let num2 = 0 // --> number
function calculadora (operacion,num1, num2) {
  switch (operacion) {
    case "suma":
      return num1 + num2
      break
    case "resta":
      return num1 - num2
      break
    case "multipli":
      return num1 * num2
      break
    case "division":
      return num1 / num2
      break
    default:
      console.error("El parametro de la variable 'operacion'  no estra en los paremetros permitidos")
  }
}
```
> A este punto no es necesario mencionarlo pero recuarda usar la consola del navegador para ejecutar los codigos 😀

Pero tambien exite `NULL` (*nulo*), el valor null es un valor especial aplicado a un puntero (o referencia) usado para indicar que no se apunta a un objeto o dato válidos. Usualmente se utiliza el valor 0 (cero) para significar null, debido a que muchos sistemas operativos consideran el intentar acceder a una dirección de memoria tan baja como un error. En resumen, null significa que el valor es *desconocido*.

## ❓ Diferencias entre `undefined` y `NULL`
En JavaScript, undefined significa que una variable ha sido declarada pero no se le ha asignado un valor. Por otro lado, null es un valor asignado que representa la ausencia intencional de cualquier objeto o valor primitivo. En resumen, undefined significa que una variable no tiene un valor asignado y null significa que una variable tiene un valor asignado pero este valor es nulo. [^1]



[^1]: [Diferencia entre null y undefiend](https://es.stackoverflow.com/questions/119964/diferencia-entre-undefined-y-null-en-javascript)
