# Algoritmos

## 📤 Ejercicio 1.
![Diagrama símbolos](images/simbolos-de-diagramas-de-flujo.png)
![Diagramas símbolos 2](images/1.png)

## Ejercicio 2

![Diagrama de Flujo Actividad ID](<images/Ejercicio 2.png>)

# Actividad 
1. Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo.

**Pseudocódigo:**
```
Inicio 
Leer A
Si A >= 1000
    Costo = 85$
Si no 
    Costo = 90
Fin si
Hacer PrecioTotal = A * Costo
Escribir "El costo total es:", PrecioTotal
Fin
```
**Diagrama de flujo:**
![Diagrama 1](<images/Diagrama Actividad ejercicio 1.png>)

**Python:**
```
cant_lapices = int(input("Ingrese la cantidad de lápices a comprar:"))
if cant_lapices >= 1000:
    total = 85 * cant_lapices
else:
    total = 90 * cant_lapices
print ("El valor a pagar es: $", total)
```

2. Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.

**Pseudocódigo:**

```
Inicio
Leer  ValorBruto
Si ValorBruto > 250000
    Descuento = ValorBruto * 0.15
Si no 
    Descuento = ValorBruto * 0.08
Fin si
ValorTotalConDescuento = ValorBruto - Descuento
Escribir "El precio final a pagar es", ValorTotalConDescuento
Escribir "El descuento total sobre su compra es:" Descuento
Fin
```

**Diagrama de flujo:**

![Diagrama 2](<images/Diagrama Actividad Ejercicio 2.png>)
Python:
(Lo hice de otra manera)

```
ValorBruto = int(input("Ingrese el Valor total de la compra:"))
if ValorBruto > 250000:
    Descuento = 0.15
else:
    Descuento = 0.08
ValorDescuento = ValorBruto * Descuento
ValorTotalConDescuento = ValorBruto - ValorDescuento
print ("El valor bruto de su compra es: $", ValorBruto)
print("El valor de la compra con descuento es:", ValorTotalConDescuento)
```

3. El director de una escuela está organizando un viaje de estudios, y requiere determinar cuánto debe cobrar a cada alumno y cuánto debe pagar a la compañía de viajes por el servicio. La forma de cobrar es la siguiente: si son 100 alumnos o más, el costo por cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de la renta del autobús es de $4000.00, sin importar el número de alumnos.

**Pseudocódigo:**
Inicio
Si alumnos 
**Diagrama de flujo:**
![Diagrama 3](<images/Diagrama Actividad Ejercicio 3.png>)

# Bucles

## Ejercicio 1
Se requiere un algoritmo para obtener la suma de diez cantidades mediante la utilización de un ciclo `while`. Realice el diagrama de flujo y el pseudocódigo.\

**Código en Python**
```py
suma = 0
cont = 1 
while cont <= 10:
    valor = int(input("Ingrese el valor": ))
    suma = suma + valor
    cont = cont + 1
print(f"La suma es:{suma}")
```

## Ejemplo 2
Se requiere un algoritmo para obtener la suma de diez cantidades mediante la utilización de un ciclo `for`. Realice el diagrama de flujo y el pseudocódigo.
**Código en Python**
```py
suma = 0
for cont in range(1,11,1):
    valor = int(input("Ingrese el valor: "))
    suma = suma + valor
print(f"La suma es: {suma}")
```
## Ejericicios del libro.
1. Un profesor tiene un salario inicial de $1500, y recibe un incremento de 10 % anual durante 6 años. ¿Cuál es su salario al cabo de 6
años? ¿Qué salario ha recibido en cada uno de los 6 años? Realice el
algoritmo y represente la solución mediante el diagrama de flujo, el
pseudocódigo y el diagrama N/S, utilizando el ciclo apropiado.

*Análisis*
1. Variables de entrada:

    - No hay.

2. Variables de salida:
    - salario:

3. Constantes:
    - salario_inicial: 1500
    - años: 6
    - incremento: 0.1

4. Otras variables
    - c

5. Ecuaciones
    - $salario = salario + (salario * incremento)$

**Pseudocódigo**
```
Inicio

salario_inicial: 1500
años: 6
incremento: 0.1

Desde c = 0 hasta c = años
    salario = salario_inicial
    Escribir "El salario del año, c, "es de", salario
    salario = salario * incremento
Fin Desde
Fin
```

**Python**
```py
salario_inicial = 1500
incremento = 0.1
años = 6
salario = salario_inicial + (salario_incial * incremento)
for c in range (1,años,1):
    print(f"El salario el año {c} es de {salario}")
    salario = salario + (salario * incremento)
print(f"El salario al cabo de los 6 años es {salario}")
```

2. “El náufrago satisfecho” ofrece hamburguesas sencillas (S), dobles
(D) y triples (T), las cuales tienen un costo de $20, $25 y $28 respectivamente. La empresa acepta tarjetas de crédito con un cargo
de 5 % sobre la compra. Suponiendo que los clientes adquieren N
hamburguesas, las cuales pueden ser de diferente tipo, realice un
algoritmo para determinar cuánto deben pagar. Represéntelo en
diagrama de flujo, pseudocódigo y diagrama N/S. 

*Análisis*
1. Variables de entrada:

    - S.
    - D.
    - T.

2. Variables de salida:
    - precio_total

3. Constantes:
    - hamburguesa_S = 20
    - hamburguesa_D = 25.
    - hamburguesa_T = 28
    - cargo = 0.05

4. Otras variables
    - N = S + D + T

5. Ecuaciones
    - $salario = salario + (salario * incremento)$

**Pseudocódigo**
```
Inicio
Leer S
```

**Python**
```
```
