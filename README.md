# Proyecto: Análisis de Datos con Python
Paginas de perfil comcretas 

import pandas as pd

# Crear un DataFrame de ejemplo
data = {
    "Producto": ["A", "B", "C", "D"],
    "Ventas": [120, 90, 150, 110]
}

df = pd.DataFrame(data)

# Mostrar datos
print("Datos:")
print(df)

# Estadísticas básicas
print("\nEstadísticas:")
print(df["Ventas"].describe())

# Producto con más ventas
top_producto = df.loc[df["Ventas"].idxmax()]
print("\nProducto con más ventas:")
print(top_producto)

