# Codigo-de-Calculo-de-Gradiente-

import math

# Função original
def f(x, y):
    return x**2 + y**2 + math.sin(x * y)

# Derivada parcial em relação a x
def dfdx(x, y):
    return 2*x + y * math.cos(x * y)

# Derivada parcial em relação a y
def dfdy(x, y):
    return 2*y + x * math.cos(x * y)

# Gradiente
def gradiente(x, y):
    return (dfdx(x, y), dfdy(x, y))

# Teste
x = 1.0
y = 2.0

g = gradiente(x, y)

print("Gradiente em (x, y) =", (x, y))
print("Resultado:", g)
