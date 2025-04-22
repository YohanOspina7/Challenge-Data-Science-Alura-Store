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

---
# Entonces... ¿Cuál tienda debería vender?

Para resolver esta pregunta me gustaría analizar los datos recogidos previamente:

No se evidencia una gran diferencia entre las ganancias de los cuatro negocios, aunque el que tuvo menos fue el negocio cuatro.
Aunque se evidencia que en cada tienda varían un poco los productos que más se venden, cada una sigue moviendo bastantes unidades. No hay mucha diferencia.

## Calificación promedio por tienda

Aunque la Tienda 1 tiene las calificaciones más bajas, no hay mucha diferencia con las demás. Todas están alrededor del 4/5, lo que indica que el servicio al cliente es bastante aceptable en general.
Costos de envío promedio por tienda

En los costos de envío se nota que la Tienda 1 tuvo costos un poco más altos, pero nada que se dispare tanto como para decir que eso esté afectando fuertemente las ventas.

## Conclusión

Aunque la Tienda 4 fue la que menos vendió, la diferencia en ingresos no es tan significativa.

Todas las tiendas venden bien, tienen buena rotación de productos, calificaciones decentes y gastos parecidos.

Entonces... ¿cuál debería vender?

En este caso, no hay una tienda que destaque negativamente al punto de tener que venderla inmediatamente. Pero si tuviera que elegir una por optimización, probablemente sería la Tienda 4, ya que es la que menos factura y su volumen de ventas tampoco la diferencia para bien.

Esto no significa que sea una mala tienda, pero si la idea es enfocar recursos, sería la menos dolorosa de soltar.

## Notas finales

Este análisis es una forma de practicar análisis exploratorio con pandas y gráficos básicos. Me ayudó a entender mejor cómo manejar datos reales y presentar la información de manera clara.
