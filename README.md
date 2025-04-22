---

# Análisis de datos de ventas

Este es un análisis de ventas realizado con Python usando pandas y matplotlib. Los datos corresponden a cuatro tiendas y vienen en archivos `.csv`. Este proyecto hace parte del primer challenge del programa de Ciencia de Datos de Alura Latam.

---

## Datos

Cada archivo tiene datos de una tienda distinta, incluyendo:

- Nombre del producto  
- Categoría  
- Precio  
- Calificación
...
---

## Objetivo

La idea principal es analizar los datos para responder lo siguiente:

- ¿Cuál tienda vendió más?
- ¿Qué categorías se venden más?
- ¿Qué tan buenas son las calificaciones por tienda?
- ¿Qué productos se venden más y cuáles menos?

---

## Facturación total

Sumé los precios de cada tienda para saber cuál tuvo más ingresos.

> Se muestra en un gráfico de barras para que sea más fácil comparar.

![imagen](https://github.com/user-attachments/assets/6319485b-4247-44a7-a7ee-120c55881a75)

---

## Ventas por categoría

Usé `.value_counts()` para saber cuántas veces aparece cada categoría.

> Se generaron gráficos de pastel por tienda, así se puede ver visualmente cuál categoría tiene más ventas.
![imagen](https://github.com/user-attachments/assets/d7d7d94b-e26e-439e-8e66-c621e5786b53)
![imagen](https://github.com/user-attachments/assets/78a47632-963c-4508-acbd-96867db57d4f)
![imagen](https://github.com/user-attachments/assets/42a6572f-7547-4777-b981-521ff88f560a)
![imagen](https://github.com/user-attachments/assets/737a8e7d-05d9-40f7-89ba-36e9eb8ddc7d)


---

## Calificación promedio

Saqué el promedio de las calificaciones por tienda con `.mean()`.

> Esto sirve para ver qué tienda tiene mejores valoraciones por parte de los clientes.

![imagen](https://github.com/user-attachments/assets/68d544a7-d735-4f6c-80e8-cadfca6b9a3c)


---

## Productos más y menos vendidos

Con `.value_counts().head(1)` y `.tail(1)` identifiqué los productos que más y menos se venden en cada tienda.

> Se muestra con un gráfico de barras horizontal.

![imagen](https://github.com/user-attachments/assets/682c8ef5-a9a9-4b26-b4a3-77356771feb9)


---

## Tecnologías usadas

- Python 3  
- pandas  
- matplotlib

---

## Cómo usar

Instala las dependencias:

```bash
pip install pandas matplotlib
```
## Notas finales

Este análisis es una forma de practicar análisis exploratorio con pandas y gráficos básicos. Me ayudó a entender mejor cómo manejar datos reales y presentar la información de manera clara.

---

¿Querés que también te ayude a organizar las carpetas del repo (`/img`, `/data`, etc.) o te creo un ejemplo de cómo subir los gráficos?
