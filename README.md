# Prácticas para la clase de Programación Analítica Descriptiva y Predictiva

## Práctica 1: Manejo de Archivos
Este proyecto consiste en un script desarrollado en **Google Colab** para analizar el archivo `mbox.txt`, extrayendo los valores numéricos de las líneas que contienen la cadena `X-DSPAM-Confidence`.  

### Objetivos  
1. Conexión al folder que contiene `mbox.txt`. 
2. Lectura del archivo y búsqueda de líneas con `X-DSPAM-Confidence`.
3. Extracción y conversión de los valores numéricos a una lista.
4. Cálculo de:  
   - Cantidad de datos extraídos.
   - Sumatoria de los valores.
   - Promedio.
   - Varianza.

### Proceso  
:one: Conexión al folder  
Se accede al archivo `mbox.txt` dentro de Google Drive.  

:two: Extracción de datos  
- Se filtran las líneas que contienen `X-DSPAM-Confidence`.  
- Se eliminan los textos no numéricos y se almacenan los valores extraídos en una lista.  

:three: Cálculo con resultados 
Se utiliza `len()` para mostrar la cantidad de datos, `sum()` para la sumatoria y **NumPy** `mean()` y `var()` para calcular el promedio y la varianza de los datos extraídos.

---

## Práctica 2: Extracción de Información con Expresiones Regulares

### Objetivos
Diseñar un código en Google Colab que permita a los estudiantes cargar el archivo `informe_acciones.txt` y extraer información clave utilizando expresiones regulares en Python.

### Proceso

:one: **Solicitud al Usuario**: Se incluyen instrucciones en el código para que el usuario cargue el archivo `informe_acciones.txt` directamente a Google Colab.

:two: Usa el módulo `re` para extraer la siguiente información:
   - **Nombre de la empresa**: Buscar el patrón del nombre en las líneas del asunto.
   - **Fecha del valor de la acción**: Encuentra el formato de fecha.
   - **Valor de la acción**: Extrae los números después de "Valor actual:".

 :three: Para cada empresa extraída, calcula:
   - Valor máximo, mínimo y promedio de los valores de la acción.

:four: Presenta los resultados de manera similar a la siguiente tabla para cada una de las empresas:
| Empresa       | Fecha       | Valor Actual | Valor Máximo | Valor Mínimo | Promedio |
|---------------|-------------|--------------|--------------|--------------|----------|
| Empresa A     | 2025-01-01  | 100          | 120          | 90           | 105      |
| Empresa B     | 2025-01-02  | 200          | 210          | 180          | 195      |

---

## Práctica 3: Creación de un arreglo y operaciones básicas

### Objetivos
Diseñar un código para crear un arreglo unidimensional de 20 elementos con valores aleatorios entre 1 y 100 y realizar los siguientes cálculos:

:one: Encontrar el valor máximo del arreglo.

:two: Encontrar el valor mínimo del arreglo.

:three: Calcular la media del arreglo.

:four: Sumar 10 a cada elemento del arreglo.

---

## Práctica 4: Manipulación de matrices

### Objetivos
En esta práctica se crearon dos matrices de 3x3 con números aleatorios entre 1 y 10.

Después de esto, se realizaron las siguientes operaciones:

:one: Sumar ambas matrices.

:two: Restar la segunda matriz de la primera.

:three: Multiplicar la primera matriz por 2.

:four: Realiza una multiplicación matricial entre las dos matrices.

---

## Práctica 5: Uso de máscaras booleanas

### Objetivos
En esta práctica se creó un arreglo unidimensional con 15 números aleatorios entre 1 y 50.

Después se realizó lo siguiente:

:one: Seleccionar los elementos mayores que 25 utilizando una máscara booleana.

:two: Contar cuántos elementos son mayores que 25.

---

## Práctica 6: Manejo de librería Pandas

### Objetivos
Para esta práctica se cargó el archivo Titanic-Dataset.csv para realizar los siguientes ejercicios:

#### :one: Ejercicio 1: Análisis de la distribución de supervivencia por combinación de sexo y clase del pasajero.
- Calcula la proporción de supervivencia para cada combinación de 'Sex' y 'Pclass'.
- Identifica qué combinación tuvo la tasa de supervivencia más alta.
- Identifica qué combinación tuvo la tasa de supervivencia más baja.

#### :two: Ejercicio 2: Identificación de familias grandes a bordo.
- Crea una nueva columna `FamilySize` sumando las columnas `SibSp` y `Parch`.
- Considera como "familia grande" a aquellas donde `FamilySize` es mayor a 3.
- Calcula el número de pasajeros en familias grandes.
- Calcula la proporción de supervivencia entre los pasajeros que pertenecen a familias grandes.

#### :three: Ejercicio 3: Segmentación por grupos de edad.
- Clasifica a los pasajeros en las siguientes categorías de edad(tip puede resultar mas sencillo realizarlo con una función)
   - Menor de Edad
   - Mayor de Edad

#### :four: Ejercicio 4: Comparación entre promedios calculados manualmente y con Pandas.
- Utiliza NumPy para calcular el promedio de las columnas `Age` y `Fare`, ignorando valores nulos.
- Compara estos valores con los promedios obtenidos utilizando los métodos nativos de Pandas.
- Verifica que los resultados sean consistentes.

#### :five: Ejercicio 5. Creación de intervalos de clase usando NumPy y análisis con Pandas.
- Divide la columna `Fare` en 5 intervalos equidistantes utilizando la función `numpy.linspace`.
- Crea una nueva columna en el DataFrame que asigne a cada pasajero el intervalo correspondiente de su tarifa.
- Calcula el número de pasajeros en cada intervalo utilizando Pandas y la proporción de supervivientes por intervalo.

---

## Práctica 7: Análisis de un Dataset con Matplotlib

### Objetivos
El objetivo de esta práctica es cargar y explorar un dataset, y luego utilizar matplotlib para crear gráficos visuales que permitan analizar e interpretar los datos.

Para este ejercicio, utilizaremos el famoso dataset Iris de la librería seaborn y visualizaremos los datos con:
- Gráfico de barras
- Histograma
- Gráfico de dispersión (scatter plot)
- Gráfico de cajas (box plot)
- Gráfico de líneas

---

## Práctica 8: Análisis de un Dataset con Seaborn y Visualización Avanzada

### Objetivos
Este ejercicio tiene como objetivo aprender a trabajar con seaborn para crear visualizaciones más avanzadas utilizando gráficos como el mapa de calor y el diagrama de violín. También, se les anima a explorar el dataset, hacer análisis descriptivos y aprender a interpretar los resultados.

#### Dataset
- Cargamos el dataset tips usando seaborn.
- Realizamos un análisis preliminar utilizando `.head()`, `.info()`, `.describe()` para obtener una visión general de los datos.
- Verificamos la existencia de valores nulos o datos faltantes.

Visualizaremos los datos con:
- Mapa de Calor (Heatmap)
- Diagrama de Violín
- Gráfico de dispersión (Scatter Plot)
- Gráfico de barras (Bar Plot)
