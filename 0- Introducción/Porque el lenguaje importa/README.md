# Porque el lenguaje importa?
El lenguaje de programación es importante porque permite a los programadores comunicarse con las computadoras y crear programas que realicen tareas específicas. Los lenguajes de programación también pueden ser más adecuados para ciertas tareas que otros, lo que puede afectar la eficiencia y la facilidad de uso del programa. [Además, algunos lenguajes de programación son más populares que otros, lo que significa que hay más recursos y herramientas disponibles para ellos.](https://www.importancia.org/lenguajes-de-programacion.php)

Ademas, ya que originalmente lo que es la programación es de la siguiente manera:
### Lenguaje de maquina
```
00110001 00000000 00000000
00110001 00000001 00000001
00110011 00000001 00000010
01010001 00001011 00000010
00100010 00000010 00001000
```
Lo cual digamos que no es muy legible para cualquiera, ya que este lenguaje es el que entiende la maquina, donde el `0` se puede interpretar como ausencia de electricidad y el `1` que si hay corriente electrica, velo de esta forma, es como apagar y prender un foco💡, cuando esta apagado es `0` y cuando esta encendido es `1`.

Aun asi seguia siendo muy dificil de aprender este `"lenguaje de programcaión"` para la mayoria de las personas, es por eso que se desarrollan los que hoy llamamos `"Compiladores"`, que es basicamente un traductor, un intermediario entre el [lenguaje de maquina](https://es.wikipedia.org/wiki/Lenguaje_de_m%C3%A1quina) y el [lenguaje ensamblador](https://es.wikipedia.org/wiki/Lenguaje_ensamblador)(que fue de los primeros lenguajes de programación), eventualmente la tecnologia se fue desarrollando más y aparecio el concepto de `"abstracción"`, usado para referirse a los niveles de complegidad de un lenguaje, por ejemplo:
### Lenguaje de maquina: nivel de abstracción = null(nulo, 0)
```
48 65 6c 6c 6f 20 6d 75 6e 64 6f 0a
```
### Lenguaje ensamblador: nivel de abstracción = low(bajo, 1)
```
section .data
    msg db 'Hola mundo',0xa
    len equ $-msg

section .text
    global _start

_start:
    mov eax,4
    mov ebx,1
    mov ecx,msg
    mov edx,len
    int 0x80

    mov eax,1
    xor ebx,ebx
    int 0x80
```
### Lenguaje C/C++: nivel de abstracción = medium(medio, 2)
```C++
#include <stdio.h>

int main() {
   printf("Hola mundo");
   return 0;
}
```
### Lenguaje JavaScript: nivel de abstracción = high(alto, 3)
```javascript
console.log("Hola mundo");
```
Aqui por acabamos de ver la legibilidad del código, que tan facil es leer el codigo segun su nivel de abstracción, donde si es más alto sera mas facil y si es más bajo sera más dificil.