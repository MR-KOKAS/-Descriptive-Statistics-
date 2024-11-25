# Proyecto de Análisis de Retornos Futuro en Empresas

Este proyecto aplica un modelo de regresión lineal para predecir retornos compuestos a futuro de empresas utilizando ratios financieros y variables de control. 

## Resumen del Proyecto
Se desarrollaron diversos modelos con el objetivo de identificar las relaciones entre características financieras y retornos futuros, categorizando empresas por tamaño (pequeñas, medianas y grandes). Adicionalmente, se exploraron términos de interacción y efectos no lineales para capturar la complejidad de las relaciones entre las variables.

### Variables Principales
- **Dependiente**:
  - `cc_return_y_f`: Retornos compuestos futuros de una empresa.
- **Independientes**:
  - Ratios financieros: `ROE`, `P/E`, `Net Profit Margin`, `Gross Margin`, `BOOKMARKET`, `EPSP`.
  - Variables categóricas: Tamaño de empresa (`Medium`, `High`).
  - Apalancamiento financiero: `fleverage`, `fleverage_squared`.

### Metodología
1. **Winsorización**: Se aplicó para mitigar el efecto de valores extremos en las variables.
2. **Análisis de Multicolinealidad**: Uso del VIF para asegurar la validez del modelo.
3. **Términos de Interacción**: Incorporación de interacciones como `EPSP_M`, `EPSP_H`, `BOOKMARKET_M`, y `BOOKMARKET_H`.
4. **Regresión Lineal**: Ajuste de varios modelos para evaluar significancia estadística y poder explicativo.

### Principales Resultados
- **Significancia**: Variables como `P/E`, `BOOKMARKET`, y `EPSP` mostraron relaciones significativas con los retornos futuros.
- **Interacciones**: Los términos de interacción permiten captar diferencias según el tamaño de la empresa.
- **Evaluación de Modelos**: El modelo final incluye términos no lineales y de interacción para maximizar la capacidad predictiva.

### Visualización
Se graficaron los retornos estimados para empresas pequeñas, medianas y grandes, mostrando las diferencias en puntos de partida (interceptos) y tendencias.

### Tecnologías Utilizadas
- Python (bibliotecas: Pandas, NumPy, Statsmodels, Matplotlib).
- Jupyter Notebook.

## Conclusiones
Este análisis ayuda a identificar factores clave que influyen en los retornos futuros de las empresas y destaca la importancia de categorizar empresas y considerar efectos no lineales para mejorar la predicción.


