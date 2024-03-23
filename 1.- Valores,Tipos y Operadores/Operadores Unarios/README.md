# 🤨 Operadores unarios
Ya que hemos visto varios de los diferentes tipos de operadores basicos, toca hablar de uno que no es un operador de simbolos como los anteriores, uno de estos es el operador `typeof`.

Este es un operador que produce un string con el nombre del tipo de valor que le demos, por ejemplo:
```JavaScript
let edad = 21
console.log(typeof edad) // --> numbre
let nombre = "Juan"
console.log(typeof nombre) // --> string
```
En los otros operadores que hemos visto hasta ahora, todos operaban en dos valores, pero typeof sola opera con un valor. Los operadores que usan dos valores son llamados operadores binarios, mientras que aquellos operadores que
usan uno son llamados operadores unarios. El operador menos puede ser usado tanto como un operador binario o como un operador unario.
```JavaScript
console.log(-(10 - 2)) // --> -8
```
Esta lección realmente es un poco corta pero es para entender el siguiente tema.
## ➕ Un pequeño PLUS-ULTRA de ![JavaScript Logo](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=white).
Aun que aun no lo entiendas bien, el operador typeof te llegara a ser muy util en algunas sircunstancias,
### Por ejemplo
Al desarrollar un programa relativamente extenso suelen ser olvidados algunas variables ya que estas se declaran al principio, y suponiendo que no quieres regresar a ver cual es el tipo de variable (numerico, string, char, etc), pues usas typeof
```JavaScript
let operacion // --> undefined
let num1 // --> undefined
let num2 // --> undefined
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
      console.error("El valor de la variable 'operacion'  no estra en los paremetros permitidos")
  }
}
```
Aquí de momento las variables declaradas no tienen ningún valor por lo que si quisieras usar typeof el valor que arrojaria seria `undefined`, ya que fueron declaradas pero no se les asigno ningun valor para que se puedan identificar, y al querer asignarle un valor no se guardara por que la variable fue declarada sin darle un tipo de valor:
```JavaScript
calculadora("suma",12,1)
typeof(num1) // undefined
```
Muy diferente a que se le asigne un tipo de valor:
```JavaScript
let operacion = "" // --> string
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
Recueda ejecutar los codigos por separado para ver su comportamiento
```JavaScript
calculadora("suma",12,1)
typeof(num1) // undefined
```