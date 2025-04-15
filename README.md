# 🛒 Challenge Alura Store Latam

Este proyecto forma parte del **Challenge de la Formación: Practicando Python para Data Science del grupo G8-ONE**, y tiene como objetivo aplicar técnicas fundamentales de **análisis y visualización de datos para obtener insights comerciales** de una serie de tiendas.

<br>

## Descripción

El objetivo principal de este challenge es **desarrollar habilidades prácticas en análisis de datos con Python**, utilizando librerías populares en el ecosistema de Data Science, como pandas, numpy, matplotlib y seaborn. A través del **análisis exploratorio de datos de ventas y productos**, se busca **identificar oportunidades, entender el comportamiento de los clientes y apoyar la toma de decisiones estratégicas**.

<br>

## Funcionalidades

- Análisis de ventas por producto, categoría y ubicación.

- Cálculo de métricas como ingresos totales, categorías de productos más y menos vendidos, calificación promedio, coste de envío promedio, entre otros.

- Visualización de datos mediante gráficos de barras.

- Manipulación de DataFrames para obtener insights relevantes.

<br>

## Uso

**1. Clonar el repositorio:**

   ```bash
   git clone https://github.com/dano796/challenge-alura-store.git
   ```

**2. Ve a Google Colab.**

**3. Haz clic en Archivo > Subir notebook y selecciona el archivo descargado.**

<br>

## Análisis Realizados

**1. Ingresos totales por tienda:** Se calcula el total de ingresos obtenidos en cada tienda.

**2. Ventas por categoría:** Se examina la cantidad de productos vendidos en cada categoría por tienda.

**3. Calificación promedio:** Se obtiene la media de las calificaciones de los productos vendidos.

**4. Productos más y menos vendidos:** Se identifican cuáles fueron los artículos más y menos vendidos en cada tienda.

**5. Costo de envío promedio:** Se analiza el valor medio del costo de envío en cada tienda.

<br>

## Ejemplo de Código

```python
def calcular_productos_por_categoria(tiendas):
    productos_por_categoria = []
    for tienda in tiendas:
        productos = tienda.groupby('Categoría del Producto')['Producto'].count().sort_values(ascending=False)
        productos_por_categoria.append(productos)
    return productos_por_categoria

productos_por_categoria = calcular_productos_por_categoria(tiendas)

for nombre, productos in zip(nombres, productos_por_categoria):
    print(f"-----------{nombre}-----------")
    print(productos)
    print()
```

---

### Practicando Python para Data Science: Challenge Alura Store

### Challenge de la Formación: Practicando Python para Data Science G8-ONE

### Daniel Ortiz Aristizábal
