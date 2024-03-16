# Reto-4
Resolver los siguientes problemas usando un notebook de python y subirlos a un repo: 

  1.Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.

```Python
numero : int
numero = int(input("Ingrese un numero entero: "))
if numero == 97:
    print('El numero ' + str(numero) + ' corresponde a la vocal "a"' )
else:
    if numero == 101:
        print('El numero ' + str(numero) + ' corresponde a la vocal "e"')
    else:
        if numero == 105:
            print('El numero ' + str(numero) + ' corresponde a la vocal "i"')
        else:
            if numero == 111:
                print('El numero ' + str(numero) + ' corresponde a la vocal "o"')
            else:
                if numero ==117:
                    print('El numero ' + str(numero) + ' corresponde a la vocal "u"')
                else:
                    print('El numero ' + str(numero) + ' no corresponde ninguna vocal')
```
  2. Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.
```Python
cadena = input("Ingrese una cadena de texto: ")
primer_caracter = cadena[0]
if primer_caracter == '0' or primer_caracter == '2' or primer_caracter == '4' or primer_caracter == '6' or primer_caracter == '8':
    print("El código ASCII del primer carácter es par.")
else:
    print("El código ASCII del primer carácter no es par.")
```
  3. Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.
```Python
Digitos = ["0","1","2","3","4","5","6","7","8","9"]
Caracter_Dado : int
Caracter_Dado = (input('Ingrese un caracter cualquiera: '))
if Caracter_Dado in Digitos:
    print('Su caracter ' + str(Caracter_Dado) + ' es un digito')
else:
    print('Su caracter ' + (str(Caracter_Dado)) + ' no es un digito')
```     
  4. Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:

    Positivo: "El número x es positivo"
    Negativo: "El número x es negativo"
    Cero (0): "El número x es el neutro para la suma"
```Python
numero_real : int
numero_real = int(input("Ingrese un numero que pertenezca a los reales: "))
if numero_real == 0:
    print('El número ' + str(numero_real) + ' es el neutro para la suma' )
else:
    if numero_real < 0:
        print('El número ' + str(numero_real) + ' es negativo' )
    else:
        if numero_real > 0:
            print('El número ' + str(numero_real) + ' es postitivo')
```
  5. Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.
```Python
Punto_Central_Circulo_Y : int
Punto_Central_Circulo_x : int
Radio_Circulo : int
Punto_x: int
Punto_y: int
Circunferencia: int
Punto_Central_Circulo_Y= int(input("Ingrese el punto en donde se ubicara el centro en y: "))
Punto_Central_Circulo_x= int(input("Ingrese el punto en donde se ubicara el centro en x: "))
Radio_Circulo= int(input("Ingrese el radio de la circunferencia: "))
Punto_x = int(input("Ingrese el punto que se desea determinar en la coordenada x: "))
Punto_y = int(input("Ingrese el punto que se desea determinar en la coordenada y: "))
distancia = ((Punto_x - Punto_Central_Circulo_x)**2 + (Punto_y - Punto_Central_Circulo_Y)**2) ** (1/2)
if distancia <= (Radio_Circulo):
    print("El punto (" + str(Punto_x)+","+ str(Punto_y)+") se encuentra en el interior de la circunferencia")
else:
    print("El punto (" + str(Punto_x)+","+ str(Punto_y)+") se encuentra afuera de la circunferencia" )
```
  6. Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.
```Python
Lado1 : int
Lado2 : int
Lado3 : int
Lado1 = int(input("Ingrese el primer lado del triangulo: "))
Lado2 = int(input("Ingrese el segundo lado del triangulo: "))
Lado3 = int(input("Ingrese el tercer lado del triangulo: "))
if (Lado1+Lado2)>Lado3:
    if (Lado2+Lado3)>Lado1:
        if(Lado3+Lado1)>Lado2:
            print("Los tres lados permiten construir un triangulo")
else:
    print("Los tres lados no permiten construir un triangulo")
```
