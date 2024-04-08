# Flujo de control.
Cuando el programa que se esta escribiendo contiene más de una declaración, estas declaraciones se ejecutan como si fueran una **"cascada"**, es decir, de arriba hacia abajo.

### Ejemplo
```javascript
let elNumero = Number(prompt("Elige un número")); //5
console.log("Tu número es la raiz cuadrada de " + elNumero * elNumero);
// Tu numero es la raiz cuadrada de 25
```
En este caso `Number` combierte la entrada del `prompt` en numero y la guarda en la variable `elNumero`, luego se imprime con el mensaje _"Tu número es la raiz cuadrada de "_, y siguiendo la logica matematica, la raiz cuadrada del cualquier número que se introdusca sera el número multiplicado por si mismo.

> [!NOTE] Porque la combersión?
> La comberción del `prompt` es necesaria ya que este solo acepta variables de tipo string (cadena) y de esa forma no es posible realizar alguna operación, es por eso que la comberción a número haciendo uso de `Number` es necesaria antes de hacer cualquier operación númerica.