# 📊 TelecomX - Predicción de Cancelación de Clientes (Churn)

## 📌 Descripción
Este proyecto forma parte del Challenge Telecom X de Alura Latam.  
El objetivo es **predecir la cancelación de clientes (churn)** en una empresa de telecomunicaciones, identificar los factores más relevantes y proponer estrategias de retención basadas en los resultados.

---

## 🛠️ Pipeline del Proyecto

1. **Preprocesamiento de Datos**
   - Eliminación de columnas irrelevantes (`customerID`).
   - Codificación de variables categóricas (`get_dummies`).
   - Verificación de proporción de churn (`value_counts`).
   - Balanceo de clases (SMOTE / oversampling).
   - Normalización/Estandarización (`StandardScaler`).

2. **Exploración**
   - Matriz de correlación.
   - Correlación directa con `Churn`.
   - Análisis dirigido (boxplots y scatter plots).

3. **Modelado Predictivo**
   - Separación de datos (train/test).
   - Modelos entrenados:
     - **Regresión Logística** (requiere estandarización).
     - **Random Forest** (no requiere normalización).

4. **Evaluación**
   - Métricas: Accuracy, Precision, Recall, F1-score.
   - Matriz de confusión.
   - Comparación crítica de modelos.

5. **Conclusiones**
   - Factores principales de churn.
   - Estrategias de retención propuestas.

---

## 📦 Dependencias
Este proyecto utiliza las siguientes librerías:
- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib

Se recomienda ejecutarlo en Google Colab, donde ya están preinstaladas.

---

## 📈 Resultados

### Comparación de Modelos

| Modelo              | Accuracy | Precision | Recall | F1-score |
|---------------------|----------|-----------|--------|----------|
| Regresión Logística | 0.97     | 0.91      | 1.00   | 0.95     |
| Random Forest       | 0.96     | 0.93      | 0.91   | 0.92     |

---

## 🔎 Conclusiones

- **Factores clave de cancelación:**
  - Contratos de corto plazo → mayor riesgo de churn.
  - Cargos mensuales elevados → clientes más propensos a cancelar.
  - Antigüedad (tenure) → clientes fieles con menor probabilidad de churn.
  - Gasto total → asociado a menor churn.

- **Estrategias de retención:**
  - Incentivar contratos de mayor duración (6+ meses).
  - Programas de fidelización para clientes antiguos.
  - Planes flexibles para clientes con facturas altas.
  - Monitoreo proactivo con modelos predictivos.

---

## 🚀 Cómo ejecutar el proyecto

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/Branhell/TelecomX_Churn_Prediction.git

## 👨‍💻 Autor
**Brayan Mejía García**  
Challenge Telecom X – Alura Latam  
[GitHub](https://github.com/Branhell)
