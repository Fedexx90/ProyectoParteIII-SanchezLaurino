# ProyectoParteIII-SanchezLaurino
Proyecto final de Visualización y Modelado Predictivo en Python. 
Hipótesis: impacto de los autos chinos en el mercado americano.

## Análisis de precios de autos en América

 🎯 Hipótesis
Analizar el impacto de los autos de origen chino en el mercado automotriz de América, comparando precios, distribución y comportamiento frente a marcas no chinas.

---

 📘 Descripción del dataset
El dataset contiene más de **550.000 registros** con información detallada de automóviles vendidos en América.  
Cada registro incluye variables como:

- **Año (`year`)**: año de fabricación del vehículo.  
- **Marca (`make`)** y **modelo (`model`)**.  
- **Condición (`condition`)** del vehículo (escala de 1 a 50).  
- **Kilometraje (`odometer`)**.  
- **Precio de venta (`sellingprice`)**.  
- **Estado (`state`)** donde se realizó la venta.  
- **Valor de mercado (`mmr`)** según la referencia Manheim Market Report.  
- Otras variables: transmisión, color, interior, vendedor, etc.

---

 🧹 Limpieza de datos
En el notebook se realizaron los siguientes pasos:
1. Eliminación de duplicados.  
2. Manejo de valores nulos: imputación o eliminación según relevancia.  
3. Estandarización de texto (por ejemplo, nombres de marcas).  
4. Filtrado de valores fuera de rango en precios y kilometraje.  
5. Conversión de la fecha de venta a formato datetime.

---

 📊 Análisis exploratorio (EDA)
- Identificación de valores perdidos.  
- Gráficos **univariados**, **bivariados** y **multivariados**.  
- Comparación de precios entre autos chinos y no chinos.  
- Distribución geográfica de ventas por estado.  
- Diagnóstico e interpretación de cada gráfico, vinculados con la hipótesis.

---

 🧠 Modelado predictivo
Se desarrolló un modelo de **regresión lineal** para estimar el precio del vehículo a partir de las variables más relevantes:

- `year`  
- `odometer`  
- `condition`  
- `is_chinese` (origen del vehículo)  
- `mmr`  

 Métricas de evaluación:
- **R² (Coeficiente de determinación)**  
- **MAE (Error Absoluto Medio)**  
- **RMSE (Raíz del Error Cuadrático Medio)**  

El modelo mostró un desempeño moderado, confirmando que las variables seleccionadas influyen en el precio, destacando el impacto negativo del origen chino en el valor promedio del vehículo.

---

 📈 Resultados principales
- Los autos chinos representan una proporción pequeña pero creciente en el mercado.  
- Su precio medio es inferior al de otras marcas, reforzando la hipótesis de una **estrategia basada en costo competitivo**.  
- El modelo predictivo demuestra que **año, odómetro y condición** son las variables más influyentes sobre el precio.  
- El **origen chino** también impacta significativamente en el valor, validando parcialmente la hipótesis inicial.

---

 💾 Dataset
El archivo original **`car_prices.csv`** supera el límite de 25 MB permitido por GitHub, por lo que se aloja externamente.

- 🔗 **Ver / abrir en Google Drive:** [car_prices.csv] https://drive.google.com/file/d/1FZZmqKXmq8iRttCYLhAKA2MxAJZowC8k/view?usp=sharing

---

 🧰 Librerías utilizadas
`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---

 📂 Estructura del repositorio

```ProyectoFinal_DS_SanchezLaurino/
├── ProyectoParteIII+SanchezLaurino.ipynb
├── README.md
└── car_prices.csv (enlace externo en Drive)```

### 🏁 Conclusión general
El estudio evidencia que los **vehículos de origen chino** han ganado una participación creciente en el mercado americano, consolidando una posición basada en "Precios Competitivos".  
El análisis predictivo confirma la relevancia de variables técnicas como el año y kilometraje, junto con el origen del vehículo, como factores determinantes en la fijación de precios.

---
