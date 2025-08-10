# Análisis de Cancelación de Clientes

## Descripción
Este repositorio contiene el análisis y los modelos predictivos desarrollados para prever la **cancelación de clientes** de un servicio. Utilizamos técnicas de machine learning para identificar los factores que más influyen en la cancelación y construir modelos para predecirla.
Es una actividad educativa, en la que se nos pide realizar estas actividades para poner en practica los visto en el curso.

## Objetivo
El objetivo principal de este análisis es identificar los **factores que afectan la cancelación de clientes** y **crear estrategias de retención** basadas en esos resultados. Los modelos predictivos desarrollados permiten prever qué clientes tienen una mayor probabilidad de cancelar su servicio.

## Metodología

### 1. **Preprocesamiento de Datos**
- **Eliminación de columnas irrelevantes**: Se eliminaron columnas como `id`, que no aportan valor predictivo.
- **Codificación de variables categóricas**: Se utilizó **OneHotEncoder** para convertir las variables categóricas a formato numérico.
- **Balanceo de clases**: Se aplicó **SMOTE** para balancear las clases y evitar el desbalanceo que afecta a la clase minoritaria (clientes que cancelan).
- **Normalización de características**: Se normalizaron las variables para los modelos que requieren esta etapa (Regresión Logística y KNN).

### 2. **Modelos**
Se entrenaron varios modelos para predecir la cancelación de clientes:
- **Regresión Logística**: Un modelo lineal que proporciona coeficientes interpretables.
- **Random Forest**: Un modelo basado en árboles que ayuda a entender la importancia de cada variable.

### 3. **Evaluación de Modelos**
Se evaluaron los modelos usando las siguientes métricas:
- **Exactitud (Accuracy)**
- **Precisión**
- **Recall**
- **F1-score**
- **Matriz de Confusión**

La **Regresión Logística** mostró un mejor desempeño en términos de **recall** para la clase 1 (cancelación), mientras que **Random Forest** mostró un buen balance entre precisión y recall.

### 4. **Análisis de la Importancia de las Variables**
Se realizó un análisis para identificar las variables más relevantes en la predicción de la cancelación:
- **Meses de contrato** y **tipo de contrato** son las variables más influyentes.
- **Cargo mensual** y **soporte técnico** también tienen un gran impacto en la retención de clientes.
- Variables como **proveedor de internet (fibra óptica)** y **TV por cable** se relacionan con una mayor probabilidad de cancelación.

### 5. **Estrategias de Retención Propuestas**
Basado en los resultados, se sugieren varias estrategias para reducir la cancelación de clientes:
- **Fidelización de clientes con contratos largos**: Promover contratos de dos años y ofrecer beneficios adicionales.
- **Mejorar el soporte técnico**: Brindar soporte adicional para clientes que tienen problemas.
- **Aumentar la carga mensual de los clientes**: Ofrecer planes premium o beneficios adicionales para justificar un cargo mensual mayor.

## Resultados
### Modelos Evaluados

#### **Regresión Logística - Resultados**
- **Exactitud**: 0.75
- **Recall (Clase 1)**: 0.79
- **F1-score (Clase 1)**: 0.63

#### **Random Forest - Resultados**
- **Exactitud**: 0.75
- **Recall (Clase 1)**: 0.73
- **F1-score (Clase 1)**: 0.61

#### **XGBoost**
Se recomendó el uso de XGBoost como modelo más robusto, pero no lo entrenamos para este proyecto.

### Importancia de las Variables
| Variable                       | Regresión Logística (Coef.) | Random Forest (Importancia) |
|---------------------------------|-----------------------------|-----------------------------|
| **Meses de contrato**           | -0.79                       | 0.17                        |
| **Tipo de contrato (2 años)**  | -0.63                       | 0.14                        |
| **Cargo mensual**               | -0.28                       | 0.13                        |
| **Proveedor de internet (fibra)**| 0.53                        | 0.07                        |
| **Soporte técnico**             | -0.18                       | 0.06                        |

---

## **Conclusiones**
- **Regresión Logística** es el modelo preferido para este caso debido a su **mejor recall** para la clase de cancelación.
- La variable más influyente es **`meses_contrato`**, seguida de **`tipo_contrato_two year`**.
- Se recomienda priorizar la fidelización de clientes con contratos largos, mejorar el soporte técnico y ofrecer servicios premium para reducir la cancelación.

---

## **Instalación**
Para ejecutar este código, necesitarás:

-  * Google Colab
-  * Cargar el data set, yo lo cargué directo en el drive para mayor comodidad, pero puedes montarlo en el espacio de trabajo de google colab, subiendo el archivo. 



