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
