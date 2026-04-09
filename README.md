
## Implementación en Python del **espectro de diseño sísmico** de la norma chilena **NCh2369:2025**.

**Autor:** MiHR <br>
**Ingeniero Civil Estructural**

---

## Descripción

Este notebook implementa el cálculo del **espectro de diseño sísmico definido en la norma chilena NCh2369:2025**, permitiendo generar de forma automática los espectros requeridos para análisis modal espectral en estructuras industriales.

El cálculo considera los parámetros fundamentales establecidos por la norma, incluyendo:

- Zona sísmica  
- Tipo de suelo  
- Factor de importancia  
- Factor de modificación de respuesta (R)  
- Razón de amortiguamiento  

A partir de estos parámetros, el script calcula:

- **Espectro de referencia**
- **Espectro de diseño reducido por el factor R**
- **Espectro de diseño vertical**, incluyendo la estimación del **coeficiente sísmico vertical** según lo indicado en la NCh2369:2025.
- **Verifica corte minimo y corte maxímo"

Como resultado, el notebook genera:

- **Un único gráfico del espectro de diseño**, que contiene simultáneamente:
  - Espectro de referencia  
  - Espectro reducido por R para dirección x
  - Espectro reducido por R para dirección y
  - Espectro vertical  

- **Archivos `.txt` con los espectros calculados**, incluyendo:
  - Espectro de referencia  
  - Espectro reducido (con R) para dirección x
  - Espectro reducido (con R) para dirección y 
  - Espectro vertical  

Estos archivos se generan en un formato compatible con software de análisis estructural como **SAP2000** o **ETABS**, permitiendo su incorporación directa como **funciones para análisis modal espectral**.

---

## Ejemplo de resultado

![Espectro de diseño](IIIZ2CR3.jpg)

---

## Ejecutar en Google Colab

Puedes ejecutar el notebook directamente en Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mihrsozs/nch2369_2025_espectro_diseno/blob/main/NCh2369_2025.ipynb)

---

## Librerías utilizadas
- numpy
- matplotlib
- pandas
- os
- csv
