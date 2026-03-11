# TelecomX_LATAM_2
Pipeline de Machine Learning para predecir el Churn de clientes en Telecom X. Incluye preprocesamiento de datos, análisis de variables y entrenamiento de modelos de clasificación (Regresión Logística, Random Forest, SMOTE).

# 📉 Telecom X – Parte 2: Predicción de Cancelación (Churn)

## 📣 Historia del Desafío
¡Felicidades! 🎉 He sido promovido después de mi excelente desempeño en el análisis exploratorio de la cancelación de clientes en Telecom X. La dedicación, claridad al comunicar los datos y visión estratégica marcaron la diferencia.

Ahora, formo parte oficial del equipo de Machine Learning de la empresa.

## 🎯 Misión
La misión de este proyecto es desarrollar modelos predictivos capaces de prever qué clientes tienen mayor probabilidad de cancelar sus servicios (Churn). La empresa busca anticiparse al problema de la cancelación mediante la construcción de un pipeline robusto para esta etapa inicial de modelado.

## 🧠 Objetivos del Desafío
- Preparar los datos para el modelado (tratamiento, codificación, normalización).
- Realizar análisis de correlación y selección de variables.
- Entrenar dos o más modelos de clasificación.
- Evaluar el rendimiento de los modelos con métricas.
- Interpretar los resultados, incluyendo la importancia de las variables.
- Crear una conclusión estratégica señalando los principales factores que influyen en la cancelación.

## 🧰 Habilidades y Prácticas Aplicadas
- ✅ Preprocesamiento de datos para Machine Learning
- ✅ Construcción y evaluación de modelos predictivos
- ✅ Interpretación de resultados y entrega de insights
- ✅ Comunicación técnica con enfoque estratégico

---

## 🛠️ Tecnologías y Herramientas Utilizadas
- **Lenguaje:** Python
- **Manipulación de Datos:** Pandas, NumPy
- **Visualización:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn (Regresión Logística, Random Forest)
- **Tratamiento de Desbalanceo:** Imbalanced-learn (SMOTE)

---

## 🚀 Pipeline del Proyecto

### 1. Preprocesamiento y Limpieza
- Carga de los datos tratados desde la Parte 1 del desafío.
- **Estandarización y Codificación:** Tratamiento de variables categóricas y aplicación de codificación necesaria para los modelos.
- **Selección de Variables:** Análisis de correlación para identificar las características con mayor impacto en la cancelación de servicios.

### 2. Entrenamiento y Evaluación de Modelos
Se evaluaron diferentes algoritmos de clasificación, analizando métricas clave como *Accuracy*, *Precision*, *Recall* y *F1-Score*, con especial atención a la clase minoritaria (clientes que cancelan).

Entre los enfoques probados se encuentran:
- Regresión Logística
- Regresión Logística con balanceo de clases
- Regresión Logística con SMOTE
- Random Forest

### 3. Resultados y Hallazgos
- Los clientes con servicios de streaming presentan un mayor riesgo de churn.
- Se requiere implementar estrategias como programas de fidelización para clientes de alto valor y un análisis profundo del uso de streaming para ajustar la oferta y mejorar la experiencia del usuario.

---

## 💡 Conclusión Estratégica

Basándonos en los resultados obtenidos, el **Modelo de Regresión Logística con balanceo de clases mediante SMOTE** es el más recomendable para predecir la cancelación de clientes, la cual ocurre principalmente en usuarios de corta permanencia y con ciertos servicios asociados. 

Este modelo mejora significativamente el *recall* de la clase “Sí” (alcanzando 0.69), permitiendo identificar a más clientes en riesgo. Sus principales ventajas radican en la interpretabilidad de los coeficientes y su alta efectividad en la detección de *churners*, incluso asumiendo algunos falsos positivos, lo cual es aceptable y preferible frente al alto costo que representa perder clientes. Este enfoque maximiza la capacidad de retención y permite a la empresa diseñar estrategias preventivas mucho más efectivas.
