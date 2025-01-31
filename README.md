# Prácticas para la clase de Programación Analítica Descriptiva y Predictiva

## 📂 Práctica 1: Manejo de Archivos
Este proyecto consiste en un script desarrollado en **Google Colab** para analizar el archivo `mbox.txt`, extrayendo los valores numéricos de las líneas que contienen la cadena `X-DSPAM-Confidence`.  

### Objetivos  
1. Conexión al folder que contiene `mbox.txt`. ✅  
2. Lectura del archivo y búsqueda de líneas con `X-DSPAM-Confidence`. ✅ 
3. Extracción y conversión de los valores numéricos a una lista. ✅
4. Cálculo de:  
   - Cantidad de datos extraídos. ✅
   - Sumatoria de los valores. ✅
   - Promedio. ✅
   - Varianza. ✅  

### Proceso  
1️⃣ Conexión al folder  
Se accede al archivo `mbox.txt` dentro de Google Drive.  

2️⃣ Extracción de datos  
- Se filtran las líneas que contienen `X-DSPAM-Confidence`.  
- Se eliminan los textos no numéricos y se almacenan los valores extraídos en una lista.  

3️⃣ Cálculo con resultados 
Se utiliza `len()` para mostrar la cantidad de datos, `sum()` para la sumatoria y **NumPy** `mean()` y `var()` para calcular el promedio y la varianza de los datos extraídos. 

