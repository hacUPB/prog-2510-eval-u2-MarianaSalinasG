# Retos y problemas

1. Se requiere obtener la distancia entre dos puntos en el plano cartesiano,
tal y como se muestra en la figura 1. Realice un diagrama de flujo y pseudocódigo que representen el algoritmo para obtener la distancia entre
esos puntos.

![alt text](images/image.webp)

## Solución:

#### *Análisis*

``Variables de entrada:``
  - y_2
  - y_1
  - x_2
  - x_1

``Variables de salida:``
- D

``Constantes:``
- No hay constantes.

``Otras variables:``
- No hay otras variables.

 ``Ecuaciones:``
- D = sqrt((y_2-y_1)^2+(x_2-x_1)^2)


#### Pseudocódigo
```
Inicio

Imprimir "Para hallar la distancia entre puntos, ingrese las coordenadas de ambos puntos"

Leer y_2
Leer y_1
Leer x_2
Leer x_1

D = sqrt((y_2-y_1)^2+(x_2-x_1)^2)
Imprimir D
Fin
```

#### Diagrama de flujo

![alt text](images/DiagramaDeFlujo_1.png)

2. Una modista, para realizar sus prendas de vestir, encarga las telas al extranjero.
Para cada pedido, tiene que proporcionar las medidas de la tela
en pulgadas, pero ella generalmente las tiene en metros. Realice un algoritmo
para ayudar a resolver el problema, determinando cuántas pulgadas
debe pedir con base en los metros que requiere. Represéntelo mediante un
diagrama de flujo y pseudocódigo (1 pulgada = 0.0254 m).

## Solución:

#### *Análisis*

``Variables de entrada:``
  - medida

``Variables de salida:``
- conversion

``Constantes:``
- pulgadas = 0.0254 m

``Otras variables:``
- No hay otras variables.

 ``Ecuaciones:``
- Conversion = medida * pulgadas

#### Pseudocódigo
```
Inicio
Imprimir "Ingrese las medidas a convertir de metros a pulgas"
Leer medida
pulgadas = 0.0254 m

Conversion = medida * pulgadas
Imprimir conversion
Fin
```

#### Diagrama de flujo

![alt text](images/DiagramaDeFlujo_2.png)

3. Se requiere determinar la hipotenusa de un triángulo rectángulo. ¿Cómo sería el diagrama de flujo y el pseudocódigo que representen el algoritmo para obtenerla? 
Recuerde que por Pitágoras se tiene que: $C^2 = A^2 + B^2$.

## Solución:

#### *Análisis*

``Variables de entrada:``
  - c1
  - c2

``Variables de salida:``
- Hipotenusa

``Constantes:``
- No hay constantes.

``Otras variables:``
- No hay otras variables.

 ``Ecuaciones:``
- Hipotenusa = sqrt(c1)^2+(c2)^2

#### Pseudocódigo
```
Inicio 
Imprimir "Ingrese el valor de los catetos del triángulo"
Leer c1
Leer c2

Hipotenusa = sqrt(c1)^2+(c2)^2
Imprimir Hipotenusa
Fin
```

#### Diagrama de flujo
![alt text](images/DiagramaDeFlujo_3.png)

4. Se requiere determinar la edad actual de una persona basándose en su fecha de nacimiento. Además, es necesario establecer si la persona ya ha cumplido años en el año en curso, si aún no lo ha hecho, o si hoy es su cumpleaños, para celebrarlo. La fecha de nacimiento y la fecha actual estarán representadas mediante tres variables: día, mes y año.

## Solución:

#### *Análisis*

``Variables de entrada:``
  - diahoy
  - meshoy
  - anohoy
  - diacumple
  - mescumple
  - anocumple

``Variables de salida:``
- edad

``Constantes:``
- No hay constantes.

``Otras variables:``
- No hay otras variables.

 ``Ecuaciones:``
- edad = anohoy - anocumple
- edad = edad - 1

#### Pseudocódigo
```
Inicio
Leer diahoy
Leer meshoy
Leer anohoy
Leer diacumple
Leer mescumple
Leer anocumple

edad = anohoy - anocumple
Si meshoy < mescumple
    edad = edad - 1
Si no si meshoy = mescumple
    Si diahoy < diacumple
        edad = edad - 1
    Si no si diahoy = diacumple
        Imprimir "Happy Birthday! 🎁"
    Si no 
        Imprimir "El usuario ya cumplió años"
    Fin si
Si no 
    Imprimir "El usuario ya cumplió años"
Fin si
Imprimir edad
Fin
```

#### Diagrama de flujo
![alt text](images/DiagramaDeFlujo_4.png)

5. Realice un algoritmo que permita determinar el sueldo semanal de un trabajador con base en las horas trabajadas y el pago por hora, considerando que a partir de la hora número 41 y hasta la 45, cada hora se le paga el doble, de la hora 46 a la 50, el triple, y que trabajar
más de 50 horas no está permitido. Represente el algoritmo mediante pseudocódigo.

## Solución:

#### *Análisis*

``Variables de entrada:``
  - sueldoSemanal
  - pagoxghora

``Variables de salida:``
- horasTrabajadas

``Constantes:``
- No hay constantes.

``Otras variables:``
- No hay otras variables.

 ``Ecuaciones:``
- sueldoSemanal = horasTrabajadas * pagoxhora
- sueldoSemanal = (40 * horasTrabajadas + (horasTrabajadas - 40) * pagoxhora * 2)
- sueldoSemanal = (40 * horasTrabajadas + (5 * horasTrabajadas * 2 ) + (horasTrabajadas - 45) * pagoxhora * 3)

#### Pseudocódigo
```
Inicio
Leer sueldoSemanal
Leer horasTrabajadas
Leer pagoxHora 

Imprimir "Ingrese el número de horas trabajadas"
Leer horasTrabajadas
Si horasTrabajadas > 50
Imprimir "No está permitido trabajar más de 50 horas"
Si no
    Si horasTrabajadas <= 40 
        sueldoSemanal = horasTrabajadas * pagoxhora
    Si no si horasTrabajadas <= 45
        sueldoSemanal = (40 * horasTrabajadas + (horasTrabajadas - 40) * pagoxhora * 2) 
    Si no si horasTrabajadas <= 50
        sueldoSemanal = (40 * horasTrabajadas + (5 * horasTrabajadas * 2 ) + (horasTrabajadas - 45) * pagoxhora * 3)
    Fin si
Fin si

Imprimir "En total su sueldo semanal es de: ", sueldoSemanal
Fin 
```

6. Se requiere un algoritmo para determinar, de N cantidades, cuántas son cero, cuántas son menores a cero, y cuántas son mayores a cero. Realice el pseudocódigo para representarlo, utilizando el ciclo apropiado.

## Solución:

#### *Análisis*

``Variables de entrada:``
  - nCantidades

``Variables de salida:``
- edad

``Constantes:``
- No hay constantes.

``Otras variables:``
- No hay otras variables.

 ``Ecuaciones:``
- edad = anohoy - anocumple
- edad = edad - 1

#### Pseudocódigo

```
Inicio
Leer nCantidades
Desde i = 1 hasta i = nCantidades
    Leer numero
    Si numero > 0
        Mayor = Mayor + 1
    Si no si numero
        Menor = Menor + 1
    Si no
        cero = cero + 1
    Fin si
Fin Desde
Imprimir " ", Mayor, ""
```

7. Se requiere un algoritmo para determinar cuánto ahorrará en pesos una persona diariamente, y en un año, si ahorra 3¢ el primero de enero, 9¢ el dos de enero, 27¢ el 3 de enero y así sucesivamente todo el año. Represente la solución mediante pseudocódigo.

## Solución:

#### *Análisis*

``Variables de entrada:``
  - diahoy
  - meshoy
  - anohoy
  - diacumple
  - mescumple
  - anocumple

``Variables de salida:``
- edad

``Constantes:``
- No hay constantes.

``Otras variables:``
- No hay otras variables.

 ``Ecuaciones:``
- edad = anohoy - anocumple
- edad = edad - 1

#### Pseucódigo

```
Inicio
ahorroxdia = 3
ahorroanual = 0
Desde i = 1 hasta i = 364 
    ahorroxdiap = ahorroxdia / 100
    Imprimir "El ahorro del día", i, "es de $", ahorroxdiap 
    ahorroxdia = 3^(c+1)
Fin Desde

ahorroanualp = (3 *(3^(i-1))) / 100
ahorroanual = ahorroanualp + ahorroxdiap

Imprimir "El ahorro total anual es de: ", ahorroanual
Fin
```

8. Realice el algoritmo para determinar cuánto pagará una persona que adquiere N artículos, los cuales están de promoción. Considere que si su precio es mayor o igual a $200 se le aplica un descuento de 15%, y si su precio es mayor a $100, pero menor a $200, el descuento es de
12%; de lo contrario, solo se le aplica 10%. Se debe saber cuál es el costo y el descuento que tendrá cada uno de los artículos y finalmente cuánto se pagará por todos los artículos obtenidos. Represente la solución mediante pseudocódigo.

```
Inicio
Leer cantidadarticulos
Leer precio
Leer descuento
Leer costoFinalxArticulo
Leer totalapagar
Leer i

totalapagar = 0
Imprimir "Ingrese la cantidad de artículos adquiridos: "
Leer cantidadarticulos
Desde i = 1 hasta i = cantidadarticulos
    Imprimir "Ingrese el precio del artículo"
    Leer precio

    Si precio >= 200
        descuento = precio * 0.15
    Si no si 100 < precio > 200
        descuento = precio * 0.12
    Si no 
        descuento = precio * 0.10
    Fin si

costoFinalxArticulo = precio - descuento
totalapagar = totalapagar + costoFinalxArticulo

Imprimir "El costo del producto sin descuento es: ", precio
Imprimir "El descuento realizado es de: ", descuento
Imprimir "El precio final del artículo con descuento es: ", costoFinalxArticulo

Fin Desde

Imprimir "El total a pagar por todos los artículos es: ", totalapagar
Fin
```

9. Realice un algoritmo y represéntelo mediante pseudocódigo para obtener una función exponencial, la cual está dada por:
    
    $𝑒^𝑥 = 1+\frac x {1!} + \frac {x^2}{2!}+ \frac {x^3}{3!}+ …$

#### Pseudocódigo

```
Inicio 
Leer bucles
Leer x
ealax = 0

Desde i = 0 hasta i = (bucles -1)
    e_n = (x^i)/(i!)
    ealax = ealax = e_n
Fin Desde
Imprimir ealax
Fin
```

10. Realice un algoritmo para obtener el seno de un ángulo y represéntelo mediante pseudocódigo. Utilice la siguiente ecuación:
$Sen x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + ...$

#### Pseudcódigo

```
Inicio
Leer bucles
Leer x
sinx = 0
n = 1

Desde i = 1 hasta i = bucles
    sini = (x^c)/(c!)
    si Residuo(i,2) = 0
        sinx = sinx - sini
    Si no 
        sinx = sinx + sini
    Fin si
    n = n + 2
Fin Desde
Imprimir sinx
Fin
```

