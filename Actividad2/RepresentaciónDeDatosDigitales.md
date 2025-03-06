# Bitácora
## Ejercicio 1

#### Pregunta 1
En la computadora se representan los datos mediante el sistema binario: 0 y 1.\
Podemos referirnos también a los estados que ellos mismos representan, mediante "combinaciones" entre los dígitos 0 y 1.

1 BIT puede representar dos estados: `0 y 1`. 
\
2 BITS pueden representar cuatro estados: `00, 01, 10 y 11`.
La fórmula para conocer la cantidad de estados que pueden representarse con ambos dígitos y el número de BITS, es: $2^n$

#### Pregunta 2
Pueden representarse como lo indica la fórmula $2^n$: dos a la N variables.

#### Pregunta 3

|Unidad|Tamaño|
|------|--------|
|Bit: Es la unidad más pequeña de información.||
|Byte|8 bits|
|Kilobyte (KB)|1,024 bytes|
|Megabyte (MB)|1,024 KB|
|Gigabyte (GB)|1,024 MB|
|Terabyte (TB)|1,024 GB|

#### Pregunta 4 
George Bool fue fundamental para la creación de, sistema booleano, mediante este principio se pueden codificar y realizar operaciones matemáticas base en el procesamiento digital.

## 📤 Ejercicio 2 - Resuelve y deja evidencia en la bitácora

- $1010101010_2$

|Posición|9|8|7|6|5|4|3|2|1|0|
|---|--|--|--|--|--|--|--|--|--|--|
|Equivalencia|512|256|128|64|32|16|8|4|2|1|
|Número binario|1|0|1|0|1|0|1|0|1|0|

$N = 512 + 128 + 32 + 8 + 2 = 682_{10} $

- $11111_2$

|Posición |4|3|2|1|0|
|--|--|--|--|--|--|
|Equivalencia|16|8|4|2|1|
|Número binario|1|1|1|1|1|

$N = 16 + 8 + 4 + 2 + 1 = 31_{10} $

- $10000000_2$

|Posición|7|6|5|4|3|2|1|0|
|--|--|--|--|--|--|--|--|--|
|Equivalencia|128|64|32|16|8|4|2|1|
|Número binario|1|0|0|0|0|0|0|0|

$N = 128 = 128_{10} $

- $100100100_2$

|Posición|8|7|6|5|4|3|2|1|0|
|--|--|--|--|--|--|--|--|--|--|
|Equivalencia|256|128|64|32|16|8|4|2|1|
|Número binario|1|0|0|1|0|0|1|0|0|

$N = 256 + 32 + 4 = 292_{10} $

-  $111000_2$

|Posición |5|4|3|2|1|0|
|--|--|--|--|--|--|--|
|Equivalencia|32|16|8|4|2|1|
|Número binario|1|1|1|0|0|0|

$N = 32 + 16 + 8 = 56_{10} $

## 📤 Ejercicio 3 

- $127_{10}$

|Posición|7|6|5|4|3|2|1|0|
|--|--|--|--|--|--|--|--|--|
|Equivalencia|128|64|32|16|8|4|2|1|
|Número binario|0|1|1|1|1|1|1|1|

$127 = 01111111_{2}$

- $246_{10}$

|Posición|8|7|6|5|4|3|2|1|0|
|--|--|--|--|--|--|--|--|--|--|
|Equivalencia|256|128|64|32|16|8|4|2|1|
|Número binario|0|1|1|1|1|0|1|1|0|

$246 = 011110110_{2}$

- $1025_{10}$

|Posición|10|9|8|7|6|5|4|3|2|1|0|
|---|---|--|--|--|--|--|--|--|--|--|--|
|Equivalencia|1024|512|256|128|64|32|16|8|4|2|1|
|Número binario|1|0|0|0|0|0|0|0|0|0|1|

$1025 = 10000000001_{2}$

- $354_{10}$

|Posición|9|8|7|6|5|4|3|2|1|0|
|---|--|--|--|--|--|--|--|--|--|--|
|Equivalencia|512|256|128|64|32|16|8|4|2|1|
|Número binario|0|1|0|1|1|0|0|0|1|0|

$1025 = 0101100010_{2}$

- $187_{10}$

|Posición|8|7|6|5|4|3|2|1|0|
|--|--|--|--|--|--|--|--|--|--|
|Equivalencia|256|128|64|32|16|8|4|2|1|
|Número binario|0|1|0|1|1|1|0|1|1|

$1025 = 010111011_{2}$

### ``Actividad de investigación y organización de resultados.``

|Tipo de dato|C|Java|Python|Características|
|---|---|---|---|---|
|Entero|int|int|int|Representa números enteros. En C y Java ocupa 4 bytes. En Python, su tamaño varía.|
|Flotante|float|float|float|Representa números decimales. En C y Java ocupa 4 bytes. En Python es de doble precisión (8 bytes).|
|Doble precisión|double|double|no existe|Similar a **float**, pero con mayor precisión. Ocupa 8 bytes en C y Java.|
|Caracter|char|char|No existe se usa **str**|Almacena un solo carácter. En C y Java ocupa 1 byte.|
|Cadena de texto|char o string|string|str|Almacena una secuencia de caracteres. En C se usa un array de char. En Java y Python es una estructura más compleja.|
|Booleano|_Bool|boolean|bool|Representa valores true o false. En C ocupa 1 byte, en Java 1 bit (pero depende de la implementación), y en Python 1 byte.|

### ``Cálculo de espacio en memoria.``

|Ejercicio de cálculo de espacio en memoria||
|--|--|
|Información|Valor en Bytes|||||||||
|Número entero|4 bytes|
|Valor flotante|4 bytes|
|Dato Booleano|1 byte|
|Un texto con 10 caracteres|10 bytes|
|Total|19 bytes|


Equivalencia: 

En $1$ $minuto$ = 6 datos.\
En $60$ $minuto$ = 360 datos.\
En $24$ $horas$ = 8640 datos.

$8640$ $datos$ $/$ $19B$ = $164160B$ $/dia$

Resultado en Kilobytes.\
$164160B$ $/$ $1024B$ = $160,3125KB$

### ``Conclusión.``
Por medio de esta actividad aprendí a diferenciar estos diferentes lenguajes de programación y entendí que cada uno maneja los datos de forma diferente pero con características similares en cuanto a almacenamiento y precisión. También me permitió conocer cómo optimizar la memoria, especialmente cuando se requiere de almacenar grandes volúmenes.

- Presición en las ordenes (indicaciones).
- Lenguaje de programación = Conjunto de reglas.
- Algoritmo = Serie de pasos precisos, sin ambigüedades, para resolver algo en específico. 
