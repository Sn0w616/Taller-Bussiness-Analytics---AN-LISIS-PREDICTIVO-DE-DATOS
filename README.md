
# Práctica de Analítica Predictiva Empresarial

## Descripción

Este proyecto corresponde al desarrollo de una práctica académica de analítica predictiva empresarial utilizando Python y Google Colab. A partir de un conjunto de datos de ventas de una empresa comercializadora de zapatos, se aplican técnicas de análisis de datos y aprendizaje automático para estudiar el comportamiento de las ventas y generar predicciones que apoyen la toma de decisiones empresariales.

## Objetivos

- Explorar y comprender el conjunto de datos.
- Realizar la limpieza y preparación de los datos.
- Identificar relaciones entre las variables comerciales.
- Implementar modelos de analítica predictiva.
- Evaluar el rendimiento de los modelos mediante métricas estadísticas.
- Interpretar los resultados y analizar su utilidad en la toma de decisiones.

## Estructura del repositorio

```text
analisis-predictivo-ventas-zapatos/
├── Practica_Analisis_Predictivo_Ventas_Zapatos.ipynb
├── S12_dataset_ventas_zapatos.xlsx
└── README.md
```

## Conjunto de datos

El archivo utilizado contiene información comercial organizada mediante las siguientes variables:

| Variable | Descripción |
|---|---|
| `Año` | Año del registro de ventas. |
| `Mes` | Mes correspondiente al registro. |
| `Presupuesto_marketing` | Presupuesto destinado al marketing. |
| `Ventas_mensuales` | Valor de las ventas mensuales. |
| `Nuevos_clientes` | Cantidad de nuevos clientes. |
| `Promociones_aplicadas` | Información sobre las promociones aplicadas. |
| `Opinion_clientes` | Variable relacionada con la opinión de los clientes. |

## Modelos implementados

### 1. Regresión lineal
Se analiza la relación entre el presupuesto de marketing y las ventas mensuales, utilizando el presupuesto como variable predictora y las ventas como variable objetivo.

**Métricas de evaluación:**
- MAE: error absoluto medio.
- RMSE: raíz del error cuadrático medio.
- R²: coeficiente de determinación.

### 2. Regresión logística
Se clasifica el cumplimiento de una meta de ventas de referencia, definida a partir de la mediana de las ventas del conjunto de datos.

Se utilizan como variables predictoras el presupuesto de marketing, los nuevos clientes, las promociones aplicadas y la opinión de los clientes.

**Métricas de evaluación:**
- Exactitud (*Accuracy*).
- Matriz de confusión.
- Informe de clasificación.
- AUC-ROC, cuando es calculable.

### 3. Árbol de decisión
Se clasifican las ventas en tres categorías: bajas, medias y altas, definidas mediante los terciles de las ventas observadas.

El modelo permite visualizar las reglas de clasificación e identificar la importancia de las variables predictoras.

**Métricas y resultados:**
- Exactitud del modelo.
- Informe de clasificación.
- Visualización del árbol.
- Importancia de las variables.

## Tecnologías utilizadas

- Python
- Google Colab
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Git y GitHub

## Ejecución del proyecto

1. Clonar o descargar este repositorio.
2. Abrir [Google Colab](https://colab.research.google.com/).
3. Importar el archivo `Practica_Analisis_Predictivo_Ventas_Zapatos.ipynb`.
4. Ejecutar las celdas del notebook en orden.
5. Cargar el archivo Excel cuando el notebook lo solicite `S12_dataset_ventas_zapatos`.
6. Revisar los análisis exploratorios, las visualizaciones, las métricas y las conclusiones obtenidas.

## Resultados esperados

Al ejecutar el notebook se obtiene:

- Análisis exploratorio y estadístico de los datos.
- Identificación de valores faltantes, duplicados e inconsistencias.
- Visualizaciones de la distribución de las ventas y su relación con el presupuesto de marketing.
- Predicciones de ventas mediante regresión lineal.
- Clasificación mediante regresión logística.
- Categorización de las ventas mediante un árbol de decisión.
- Comparación del rendimiento de los modelos.
- Interpretación de los resultados y conclusiones de la práctica.

## Consideraciones

- El conjunto de datos tiene un tamaño limitado, por lo que los resultados deben interpretarse con precaución.
- Los años que presenten valores atípicos deben verificarse con la fuente original.
- La mediana de las ventas se utiliza como umbral de referencia para la regresión logística; no representa necesariamente una meta empresarial oficial.
- Los modelos permiten identificar patrones y relaciones, pero no demuestran por sí solos causalidad entre las variables.
- Los resultados numéricos se obtienen al ejecutar el notebook.

## Referencias

- Google Cloud. (s.f.). What is predictive analytics? https://cloud.google.com/learn/what-is-predictive-analytics?hl=es
- Scikit-learn. [Documentación oficial](https://scikit-learn.org/stable/).

## Autoría

Proyecto desarrollado con fines académicos en el marco de actividades de formación para el curso de Bussiness Analytics en la Especialización en analítica y ciencia de datos.

