## Ejercicios en código en Python

1. Se requiere obtener la distancia entre dos puntos en el plano cartesiano,
tal y como se muestra en la figura 1. Realice un diagrama de flujo y pseudocódigo que representen el algoritmo para obtener la distancia entre
esos puntos.

**Pseudocódigo**
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
### Desarrollo código en Python

```py
def calculo_de_distancia():
    x_1 = float(input("Ingrese la coordenada x del primer punto: "))
    y_1 = float(input("Ingrese la coordenada y del primer punto: "))
    x_2 = float(input("Ingrese la coordenada x del segundo punto: "))
    y_2 = float(input("Ingrese la coordenada y del segundo punto: "))
    
    D = math.sqrt ((y_2 - y_1) ** 2 + (x_2 - x_1) ** 2)
    print("La distancia entre los puntos es: {D}")
```

2. Una modista, para realizar sus prendas de vestir, encarga las telas al extranjero.
Para cada pedido, tiene que proporcionar las medidas de la tela
en pulgadas, pero ella generalmente las tiene en metros. Realice un algoritmo
para ayudar a resolver el problema, determinando cuántas pulgadas
debe pedir con base en los metros que requiere. Represéntelo mediante un
diagrama de flujo y pseudocódigo (1 pulgada = 0.0254 m).

**Pseudocódigo**
```
Inicio
Imprimir "Ingrese las medidas a convertir de metros a pulgas"
Leer medida
pulgadas = 0.0254 m

Conversion = medida * pulgadas
Imprimir Conversion
Fin
```
### Desarrollo código en Python

```py
def conversion_de_medidas():
    print("Ingrese las medidas a convertir de metros a pulgadas")
    medida = float(input("Ingrese la medida en metros"))

    pulgadas = 0.0254 
    conversion = medida * pulgadas 

    print("La medida en pulgadas es de:" {conversion})
```

3. Se requiere determinar la hipotenusa de un triángulo rectángulo. ¿Cómo sería el diagrama de flujo y el pseudocódigo que representen el algoritmo para obtenerla? 
Recuerde que por Pitágoras se tiene que: $C^2 = A^2 + B^2$.

**Pseudocódigo**

```
Inicio 
Imprimir "Ingrese el valor de los catetos del triángulo"
Leer c1
Leer c2

Hipotenusa = sqrt(c1)^2+(c2)^2
Imprimir Hipotenusa
Fin
```

### Desarrollo código en Python

```py
def calculo_de_hipotenusa():
    print("Ingrese el valor de los catetos del trángulo")
    c1 = float(input("Ingrese el valor del cateto 1"))
    c2 = float(input("Ingrese el valor del cateto 2"))

    hipotenusa = math.sqrt(c1**2 + c2**2)
    print("La hipotenusa del triángulo es:"{hipotenisa})
```

4. Se requiere determinar la edad actual de una persona basándose en su fecha de nacimiento. Además, es necesario establecer si la persona ya ha cumplido años en el año en curso, si aún no lo ha hecho, o si hoy es su cumpleaños, para celebrarlo. La fecha de nacimiento y la fecha actual estarán representadas mediante tres variables: día, mes y año.

**Pseudocódigo**
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

### Desarrollo código en Python

```py
def calcular_la_edad():
    diahoy = int(input("Ingrese el día de hoy: "))
    meshoy = int(input("Ingrese el mes de hoy: "))
    anohoy = int(input("Ingrese el año de hoy: "))
    diacumple = int(input("Ingrese el día de su cumpleaños: "))
    mescumple = int(input("Ingrese el mes de su cumpleaños: "))
    anocumple = int(input("Ingrese el año de su cumpleaños: "))
    
    edad = anohoy - anocumple
    if meshoy < mescumple:
        edad = edad - 1
    elif meshoy == mescumple:
        if diahoy < diacumple:
            edad = edad - 1
        elif diahoy == diacumple:
            print("Happy Birthday! 🎁")
        else:
            print("El usuario ya cumplió años")
    else:
        print("El usuario ya cumplió años")

    print("La edad del usuario es:" {edad})
```

5. Realice un algoritmo que permita determinar el sueldo semanal de un trabajador con base en las horas trabajadas y el pago por hora, considerando que a partir de la hora número 41 y hasta la 45, cada hora se le paga el doble, de la hora 46 a la 50, el triple, y que trabajar
más de 50 horas no está permitido. Represente el algoritmo mediante pseudocódigo.

**Pseudocódigo**
```
Inicio
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

### Desarrollo código en Python

```py
def calcular_el_sueldo():
    pagoxHora = float(input("Ingrese el pago por hora: "))
    horasTrabajadas = int(input("Ingrese el número de horas trabajadas: "))

    if horasTrabajadas > 50:
        print("No está permitido trabajar más de 50 horas")
    else:
        if horasTrabajadas <= 40:
            sueldoSemanal = horasTrabajadas * pagoxHora
        elif horasTrabajadas <= 45:
            sueldoSemanal = (40 * pagoxHora + (horasTrabajadas - 40) * pagoxHora * 2)
        elif horasTrabajadas <= 50:
            sueldoSemanal = (40 * pagoxHora + (5 * pagoxHora * 2) + (horasTrabajadas - 45) * pagoxHora * 3)
        
        print("El sueldo semanal es:"{sueldoSemanal})
```