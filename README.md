#CONVERSOR DE DECIMAL A BINARIO

Este código permite que el programa realice conversiones de números **decimales** a **binarios**.

Facilidades del programa:
* **Conversión automática** de un número decimal cualquiera.
* **Mayor velocidad** que el cálculo convencional.
* **Mayor exactitud** sin opción a error de cálculo.

```python
def dec2bin(numero_decimal, numero_bits):
    numero_binario = bin(numero_decimal)
    if numero_decimal >= 0:
            numero_binario = numero_binario[2:len(numero_binario)]
            # quita el "0b" del principio
    
        while len(numero_binario) < numero_bits:
            # añade 0's a la izquierda si hace falta
            numero_binario = "0" + numero_binario

        else:
        numero_binario = numero_binario[3:len(numero_binario)]
        # quita el "-0b" del principio
        while len(numero_binario) < numero_bits:
            # añade 1's a la izquierda si hace falta
            numero_binario = "1" + numero_binario
    return numero_binario
```
![Imagen de código binario](https://extraconfidencial.com/wp-content/uploads/2021/02/codigo_binario.jpg)
