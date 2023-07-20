# Python

# 1. PEP8
Mencione 3 normas pertenecientes a la guía de estilos PEP8 y brinde
ejemplos de su uso e importancia.

## [Espacios, no Tabs](https://peps.python.org/pep-0008/#tabs-or-spaces)
El uso de espacios en lugar de tabuladores asegura que el código se vea igual en diferentes editores y entornos, evitando problemas de formato.
```python
def foobar():
    if True:
        resultado = 10
    else:
        resultado = 5
```

## [Nombres de variables](https://peps.python.org/pep-0008/#descriptive-naming-styles)
El uso de nombres descriptivos en minúsculas con guiones bajos mejora la legibilidad y comprensión del código. Ayuda a otros desarrolladores a entender el propósito y la función de una variable o función simplemente leyendo su nombre.
```python
registros_faltantes = 10

generar_reportes()
```

## [longitud de línea a 79 caracteres](https://peps.python.org/pep-0008/#maximum-line-length)
Limitar la longitud de línea ayuda a mantener el código legible sin necesidad de desplazarse horizontalmente. También facilita la visualización del código en pantallas o entornos con espacios reducidos. Si una línea excede los 79 caracteres, es recomendable dividirla o reestructurar el código para que sea más legible.
```python
data = [ventas, compras reportes]
```



# 2. Datos mutables de Python
En Python, los tipos de datos mutables son aquellos que permiten cambiar o modificar sus elementos después de haber sido creados, los valores contenidos en estos tipos de datos pueden ser alterados sin necesidad de crear un nuevo objeto. Ejemplo `my_list = [1, 2, 3]`, `my_dict = {"nombre": "Chispa", "color": "cafe"}`, ``.



# 3. Datos inmutables de Python
En Python, los tipos de datos inmutables son aquellos cuyos valores no pueden ser modificados una vez que han sido creados. Ejemplo, `my_tuple = (1, 2, 3)`



# 4. Complete el siguiente programa
```python

x = 6
if x < 0:
    print("negativo")
elif x == 0:
    print("cero")
else:
    print("positivo")

```

# 5. ¿Cuál de las opciones es equivalente al código de Python mostrado?
Respuesta, D. `print(“Si”) if 5 == 2 else print(“No”)``