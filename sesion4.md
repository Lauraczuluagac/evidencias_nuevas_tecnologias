<!-- No borrar o modificar -->
[Inicio](./index.md)

# Actividades Sesión 4

### Actividad: Resolver utilizando funciones en Python

1. Calculadora Básica: Crea una función llamada calculadora que tome tres argumentos: dos números y un operador (+, -, *, /). La función debe realizar la operación indicada en los dos números y devolver el resultado.

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







