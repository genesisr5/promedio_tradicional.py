def ingresar_datos_diarios(dias_semana):
  """Ingresa las temperaturas diarias para una semana.

  Args:
    dias_semana: Número de días de la semana.

  Returns:
    Una lista con las temperaturas diarias.
  """

  temperaturas = []
  for dia in range(dias_semana):
    temperatura = float(input(f"Ingrese la temperatura del día {dia+1}: "))
    temperaturas.append(temperatura)
  return temperaturas

def calcular_promedio(temperaturas):
  """Calcula el promedio de una lista de temperaturas.

  Args:
    temperaturas: Una lista de temperaturas.

  Returns:
    El promedio de las temperaturas.
  """

  return sum(temperaturas) / len(temperaturas)

# Obtener los datos de entrada
dias_semana = 7
temperaturas = ingresar_datos_diarios(dias_semana)

# Calcular y mostrar el promedio
promedio = calcular_promedio(temperaturas)
print(f"El promedio semanal de temperatura es: {promedio:.2f} °C")
