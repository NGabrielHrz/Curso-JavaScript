# 🤨 Converción de tipo automática
JavaScript tiende a salirse de su camino para aceptar casi cualquier programa que le demos, incluso programas que hacen cosas extrañas. Esto es bien demostrado por las siguientes expresiones:
```javascript
console.log(8 * null) // → 0
console.log("5" - 1) // → 4
console.log("5" + 1) // → 51
console.log("cinco" * 2) // → NaN
console.log(false === 0) // → true
```
Cuando un operador es aplicado al tipo de valor “incorrecto”, JavaScript silenciosamente convertirá ese valor al tipo que necesita, utilizando una serie de reglas que frecuentemente no dan el resultado que quisieras o esperarías. Esto es llamado *correción de tipo*. En la primera expreción podemos ver que un número es multiplicado por un null, como ya se vio antes, el `null` para la maquina tiene el valor de 0, por lo que JavaScript intenta realizar una multiplicación por lo que el resultado es cero.
```javascript
console.log(8 * null) // → 0
```

Para la segunda expresión, el "5" es un string, no un número, pero Javascript intenta realizar la operación, por lo que termina combirtiendo el string en un número, como resultado da 4.
```javascript
console.log("5" - 1) // → 4
```
Para tercera expresión, el singno de + tiene diferentes funciones, y una de estas es la concatenación, utilzada principalmente para unir dos cadenas de texto del tipo string, y en este caso, teine prioridad la concatenación antes que la suma, por lo que combertira el número 1 en string y los juntara.
```javascript
console.log("5" + 1) // → 51
```
Para la cuarta expresión la palabra "cinco" no se puede traducri a número, pero la maquina entinden que se tiene que ralizar una multiplicación, por lo que combierte la palabra a un `NaN` y al multiplicarlo da como resultado `NaN`.
```javascript
console.log("cinco" * 2) // → NaN
```
Para la quinta expresión, cuando se utiliza === para comparar valores del mismo tipo, el desenlace es fácil de predecir: debemos de obtener verdadero cuando ambos valores son lo mismo, excepto en el caso de NaN. Pero cuando los tipos difieren, JavaScript utiliza una serie de reglas complicadas y confusas para determinar que hacer. En este caso en especial es un poco curioso, ya que de una u otra forma JavaScript interpreta que `false` es igual a 0, que por cierto, de una u otra forma logica, false si equivale a 0 para la maquina pero no para nosotros.
```javascript
console.log(false === 0) // → true
```
## 🧑‍🏫 Tema a comprender
Es muy común que al principio te confundas mucho, pero puesto de otra manera, *no mescles peras con mazanas*, dicho de esa forma para que recuerdes que si intentas realizar una operación u obtención de algun dato con tipos de datos diferentes, javascript lo interpretara de otra forma.

Practica diferentes expreciones con los diferentes tipos de datos ya antes vistos para ver como reacciona JavaScript y entender un poco mejor las consecuencias que puede traer a futuro en un programa.