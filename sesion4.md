<!-- No borrar o modificar -->
[Inicio](./index.md)

# Actividades Sesión 4

### Actividad: Resolver utilizando funciones en Python

- 1. Calculadora Básica: Crea una función llamada calculadora que tome tres argumentos: dos números y un operador (+, -, *, /). La función debe realizar la operación indicada en los dos números y devolver el resultado.

```
def calculadora(n1,n2,op):
    resultado=0
    if op=='+':
        resultado = n1 + n2
    elif op=='-':
        resultado = n1 - n2
    elif op=='*':
        resultado = n1 * n2
    elif op=='/':
        resultado = n1 / n2 
        
    return resultado 

n1=int(input("ingresse un numero"))                  
n2=int(input("ingresse un segundo numero"))                  
op=input("ingresse un operador")                 
x=calculadora(n1,n2,op)  
print(x)
```

- 2. Conteo de Vocales: Crea una función llamada contar_vocales que tome una cadena como argumento y devuelva el número de vocales (a, e, i, o, u) que contiene la cadena.

``` 
def contar_vocales(cadena):
    contador = 0
    cadena = cadena.lower()
    for letra in cadena:
        if letra in "aeiou":
            contador += 1
    
    return contador

cadena = "diego"
resultado = contar_vocales(cadena)
print(f"El número de vocales en la cadena es: {resultado}")

```

- 3. Primo o No Primo: Escribe una función llamada es_primo que tome un número entero positivo como argumento y determine si es un número primo (es decir, solo es divisible por 1 y por sí mismo). La función debe devolver True si es primo y False si no lo es.

```
def es_primo(numero):
    if numero <= 1:
        return False
    
    for i in range(2, int(numero**0.5) + 1):
        if numero % i == 0:
            return False
    
    return True

numero = 12  
resultado = es_primo(numero)

if resultado:
    print(f"{numero} True.")
else:
    print(f"{numero} False.")

```

- 4. Contador de Palabras: Escribe una función llamada contar_palabras que tome una cadena como argumento y devuelva el número de palabras en esa cadena. Supón que las palabras están separadas por espacios.

```
def contar_palabras(cadena):
    palabras = cadena.split()
    numero_de_palabras = len(palabras)
    return numero_de_palabras

cadena = "Esto es una cadena de ejemplo"
resultado = contar_palabras(cadena)
print(resultado)

```




