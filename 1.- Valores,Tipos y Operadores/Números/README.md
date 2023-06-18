# 🧮 Números
Puede pareces algo redundante explicar los numeros a estas alturas, ya que aquí, en España, o en China, los números siguen siendo números, y el como se representa en JavaScript es muy similar a la vida cotidiana:
```javascript
13
```
Así, ya si quieres usarlo para una suma por ejemplo, quedaria algo así:
```javascript
12+1
```
Si lo que quieres es introducir tú tus propios valores pues hay que ponerle más producción, y una *funcion*, algo así:
### Suma
```Javascript
function suma(num1,num2) { // La función tomara los argumentos que les proporciones al llamar a la función
  console.log(num1+num2); // Imprime la suma de num1 y num2
}

suma(12,1) //Manda a llamar a la función, y toma los parametros que le proporcionamos.
```
Tambien se pueden realizar otro tipo de operaciones:
### Resta
```Javascript
function suma(num1,num2) { // La función tomara los argumentos que les proporciones al llamar a la función
  console.log(num1-num2); // Imprime la resta de num1 y num2
}

suma(14,1) //Manda a llamar a la función, y toma los parametros que le proporcionamos.
```
### Multiplicación
```Javascript
function suma(num1,num2) { // La función tomara los argumentos que les proporciones al llamar a la función
  console.log(num1*num2); // Imprime la multiplicación de num1 y num2
}

suma(13,1) //Manda a llamar a la función, y toma los parametros que le proporcionamos.
```
### Divición
```Javascript
function suma(num1,num2) { // La función tomara los argumentos que les proporciones al llamar a la función
  console.log(num1/num2); // Imprime la suma de num1 y num2
}

suma(13,1) //Manda a llamar a la función, y toma los parametros que le proporcionamos.
```
De momento, esto es todo lo que hay que explicar de los números, como declararlos y realizar operaciones aritmeticas con ellos, basicamente todo lo que hemos visto de ellos desde la primaria.

## ➕ Un pequeño PLUS-ULTRA
Aqui te dejo un ejemplo para poder calcualar el area de un circulo:
```javascript
const PI = 3.1415926;

function AreaCirculo(r) {
  console.log(PI * Math.pow(r, 2));
}

AreaCirculo(5);
```
Diviertete con el😁.