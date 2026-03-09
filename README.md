# PT2_Alura_TelecomX_Challenge

## 📝 Descripción del Proyecto
Este proyecto de ciencia de datos tiene como finalidad analizar y predecir la cancelación del servicio (Churn) de los clientes de la empresa de telecomunicaciones **TelecomX**.  

El propósito principal es identificar cuáles variables influyen con mayor peso en la decisión de un cliente de abandonar el servicio. Con base en este análisis, se desarrolla un modelo de **machine learning** capaz de estimar qué clientes presentan mayor probabilidad de cancelar su suscripción.

---

## 🛠️ Tecnologías y Librerías Utilizadas

- **Python** – Lenguaje principal utilizado para el desarrollo del análisis.
- **Pandas** – Herramienta para la manipulación y procesamiento de datos.
- **NumPy** – Librería utilizada para cálculos y operaciones numéricas.
- **Scikit-learn** – Utilizada para construir, entrenar y evaluar los modelos de aprendizaje automático.
- **Matplotlib** y **Seaborn** – Empleadas para la visualización de datos y el análisis exploratorio (EDA).

---

## 📊 Conjunto de Datos

El análisis se realizó utilizando el archivo **`datos_tratados.csv`**, generado en la primera etapa del proyecto. Este conjunto de datos contiene información detallada sobre los clientes de TelecomX, incluyendo:

**Datos del cliente**
- Género
- Edad
- Estado civil (pareja)
- Dependientes

**Servicios contratados**
- Tipo de conexión a internet (DSL o fibra óptica)
- Líneas telefónicas múltiples
- Servicios adicionales como seguridad en línea, respaldo, entre otros.

**Información de la cuenta**
- Antigüedad del cliente (tenure)
- Tipo de contrato
- Facturación mensual
- Facturación total
- Método de pago

---

## 🤖 Modelos de Machine Learning y Resultados

Durante el desarrollo del proyecto se implementaron diversos **modelos de clasificación** con el objetivo de determinar cuál ofrecía mejor desempeño en la predicción del churn.

De acuerdo con la métrica **ROC AUC Score**, los modelos que mostraron mejores resultados fueron:

- **Naive Bayes Gaussiano**
- **Regresión Logística**

La métrica ROC AUC resulta especialmente adecuada en este caso, ya que los conjuntos de datos relacionados con churn suelen presentar **desbalance entre las clases**.

---

## 🔑 Factores Principales Asociados al Churn

El análisis del comportamiento de los modelos permitió identificar las variables que tienen mayor influencia en la cancelación del servicio:

- **Tipo de contrato:** Los clientes con contratos mensuales presentan mayor probabilidad de abandonar el servicio.
- **Antigüedad del cliente (Tenure):** Los clientes con menor tiempo en la empresa tienen mayor riesgo de churn.
- **Tipo de servicio de internet:** Se observó una mayor tasa de cancelación entre quienes utilizan fibra óptica.
- **Método de pago:** El uso de cheque electrónico está asociado a un mayor nivel de abandono.

---

## 💡 Conclusiones y Recomendaciones

Los modelos desarrollados lograron ofrecer un buen desempeño en la identificación de clientes con riesgo de cancelación. Además, el análisis de las variables más relevantes proporciona información valiosa para la toma de decisiones estratégicas.

Con base en los resultados obtenidos, TelecomX podría considerar las siguientes acciones:

- Implementar **estrategias de retención** dirigidas a clientes nuevos y a aquellos con contratos mensuales.
- Analizar y mejorar posibles problemas en el **servicio de internet por fibra óptica**.
- Evaluar la experiencia de los clientes que utilizan **cheque electrónico como método de pago**.

Estas medidas podrían contribuir a **reducir la tasa de cancelación y mejorar la fidelización de clientes**.
