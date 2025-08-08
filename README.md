# Análisis de Evasión de Clientes (Churn) en Telecomunicaciones

---

## 🚀 Propósito del Análisis

Este proyecto se enfoca en comprender y mitigar la **evasión de clientes (Churn)** en una empresa de telecomunicaciones. El Churn es un desafío crítico, ya que **retener a un cliente existente es significativamente más rentable que adquirir uno nuevo**.

Mi objetivo principal fue:
* Identificar los **factores clave** que influyen en la decisión de un cliente de cancelar sus servicios.
* Extraer **insights accionables** que permitan a la empresa desarrollar estrategias de retención más efectivas y personalizadas.

Los datos utilizados provienen de un conjunto de información de clientes de una compañía de telecomunicaciones, accesible en el siguiente enlace: [TelecomX_Data.json](https://github.com/ingridcristh/challenge2-data-science-LATAM/blob/main/TelecomX_Data.json).

---

## 📂 Estructura del Proyecto y Organización de Archivos

El proyecto está organizado de forma clara para facilitar su comprensión y reproducción:

* **`Challenge_telecom_x.ipynb`**: Este es el cuaderno principal de Jupyter/Colab que contiene todo el proceso de análisis, desde la carga y limpieza de datos hasta el análisis exploratorio y la generación de *insights*. Puedes acceder a él directamente aquí: [Challenge_telecom_x.ipynb](https://github.com/CrystyGzz/Challenge-telecom-x/blob/main/Challenge_telecom_x.ipynb)
* **`README.md`**: Este archivo de documentación que estás leyendo, proporcionando una visión general del proyecto.

---

## 📊 Ejemplos de Gráficos e Insights Clave

Durante el análisis exploratorio de datos (EDA), descubrí patrones cruciales que revelan el perfil del cliente propenso a la evasión:

### Distribución de Churn
El dataset presenta un **desequilibrio de clases**, con aproximadamente 25.7% de clientes que no rotan** frente a un 74.3% que sí lo hace**. Esto es fundamental para futuras etapas de modelado.
<img width="642" height="661" alt="download" src="https://github.com/user-attachments/assets/717bac6b-90c5-40dd-af57-7b91b7235223" />
<img width="630" height="478" alt="download" src="https://github.com/user-attachments/assets/7ad37a5b-4bff-4209-8357-bd6edfd19f68" />


### Influencia de Variables Categóricas
* **Tipo de Contrato:** Los clientes con **contratos "Mes a Mes"** muestran una tasa de rotación notablemente superior en comparación con aquellos con contratos anuales o bianuales. Esto sugiere una menor lealtad y mayor flexibilidad para cambiar de proveedor.
* **Servicio de Internet:** La presencia de **"Fibra Óptica"** se asocia con una mayor propensión a la rotación, lo que podría indicar insatisfacción con el servicio o el costo percibido.
* **Método de Pago:** El uso de **"Cheque Electrónico"** también se correlaciona con una tasa de Churn más alta.
<img width="888" height="590" alt="download" src="https://github.com/user-attachments/assets/f11fde25-5b5b-4aaa-b99b-848a489f9341" />
<img width="888" height="590" alt="download" src="https://github.com/user-attachments/assets/5c449222-30ad-47a9-9776-e58777a96f0d" />
<img width="888" height="590" alt="download" src="https://github.com/user-attachments/assets/3a163252-cf08-4ddc-bf83-26c6a6298107" />
<img width="888" height="590" alt="download" src="https://github.com/user-attachments/assets/fc60eb0e-43d0-47b4-99ab-434e07c198b6" />
<img width="888" height="590" alt="download" src="https://github.com/user-attachments/assets/3abdc311-3699-441a-94c5-ddd44d99d5f1" />


### Influencia de Variables Numéricas
* **Antigüedad del Cliente (`Antiguedad_Meses`):** Los clientes que rotan tienden a tener una **antigüedad significativamente menor** en el servicio. Esto resalta que los **clientes nuevos son más vulnerables** a la evasión.
* **Cargos Mensuales (`Cargos_Mensuales`):** Se observó que los clientes con **cargos mensuales muy altos**, y en algunos casos también muy bajos, tienen una mayor probabilidad de rotar, lo que sugiere una posible insatisfacción con el precio/valor percibido.
<img width="846" height="553" alt="download" src="https://github.com/user-attachments/assets/64633515-8652-4200-8f5c-ce0077f9480d" />
<img width="867" height="552" alt="download" src="https://github.com/user-attachments/assets/e1055b0e-9c54-46d8-86bc-2c56402c4301" />
<img width="854" height="553" alt="download" src="https://github.com/user-attachments/assets/cd62342a-5061-46f9-bc9b-475dfc26b6f0" />




---

## 🛠️ Instrucciones para Ejecutar el Notebook

Para explorar y replicar este análisis, sigue estos pasos:

1.  **Abrir en Google Colab:** La forma más sencilla es abrir directamente el archivo `Challenge_telecom_x.ipynb` en Google Colab. Puedes hacerlo haciendo clic en el archivo en GitHub y luego seleccionando "Open in Colab" (Abrir en Colab) en la parte superior.
2.  **Ejecutar Celdas:** Una vez abierto en Colab, puedes ejecutar cada celda secuencialmente (Ctrl+Enter o el botón de "Reproducir" en cada celda).
3.  **Entorno de Ejecución:** Asegúrate de que tu entorno de ejecución de Colab esté configurado para Python 3. Todas las librerías necesarias (Pandas, Matplotlib, Seaborn) están preinstaladas en Colab.
4.  **Datos:** El notebook carga los datos directamente desde la URL de GitHub proporcionada al inicio del análisis, por lo que no necesitas descargar el archivo `TelecomX_Data.json` localmente.

---
