# 📊 Análisis de Evasión de Clientes (Churn) — Telecom X

## 📌 Descripción del proyecto

Este proyecto analiza la **evasión de clientes (Churn)** en una empresa ficticia de telecomunicaciones llamada **Telecom X**.

El objetivo es identificar **patrones y factores que influyen en la cancelación del servicio**, utilizando técnicas de **Análisis Exploratorio de Datos (EDA)**.

Durante el análisis se aplican procesos de:

- extracción de datos
- limpieza y transformación
- análisis exploratorio
- visualización de datos
- generación de insights
- recomendaciones estratégicas

Este proyecto forma parte de un desafío de **Data Science orientado al análisis de comportamiento de clientes**.

---

# 🎯 Objetivos del análisis

El objetivo principal del proyecto es identificar **factores asociados con la evasión de clientes**, tales como:

- características demográficas
- tipo de contrato
- método de pago
- servicios contratados
- gasto mensual
- antigüedad del cliente

A partir de este análisis se generan **insights y recomendaciones estratégicas** para mejorar la retención de clientes.

---

# 🧰 Tecnologías utilizadas

Este proyecto fue desarrollado utilizando Python y herramientas de análisis de datos.

Principales tecnologías:

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook / Google Colab**

---

# 📂 Estructura del proyecto

```

📁 TelecomX_LATAM
│
├── 📄 TelecomX_LATAM.ipynb   # Notebook con todo el análisis
├── 📄 README.md              # Documentación del proyecto
│
└── 📁 data
└── telecom_churn.json        # Dataset utilizado

````

---

# 🔎 Proceso de análisis

El proyecto sigue un flujo de análisis basado en el modelo **ETL (Extract, Transform, Load)** y posteriormente **EDA**.

## 1️⃣ Extracción de datos (Extract)

Los datos se obtienen desde una **API en formato JSON**, que contiene información de clientes, servicios contratados y facturación.

Los datos son cargados y convertidos a un **DataFrame de Pandas** para su procesamiento.

---

## 2️⃣ Exploración inicial del dataset

Se analizó la estructura general del dataset:

- dimensiones del dataset
- tipos de datos
- nombres de columnas
- estructura de registros

Esto permitió detectar **columnas con estructuras anidadas provenientes del JSON**.

---

## 3️⃣ Transformación y limpieza de datos (Transform)

Se realizaron varios procesos de preparación:

- normalización de columnas anidadas
- unificación de información en un único DataFrame
- revisión de valores nulos
- detección de duplicados
- corrección de tipos de datos
- limpieza de variables categóricas

---

## 4️⃣ Creación de nuevas variables

Se generaron variables adicionales para enriquecer el análisis:

- **Cuentas_Diarias** → gasto mensual dividido por 30
- **Cantidad_Servicios** → número total de servicios contratados por cliente

---

## 5️⃣ Estandarización de datos

Se realizaron mejoras en el dataset para facilitar el análisis:

- renombrado de columnas
- conversión de variables binarias a **0 y 1**
- estandarización de variables categóricas

---

# 📊 Análisis Exploratorio de Datos (EDA)

Se analizaron diferentes variables relacionadas con la evasión de clientes.

## Distribución de churn

Se estudió la proporción de clientes que cancelan el servicio.

Resultados:

- **73% de clientes permanecen**
- **26% de clientes cancelan**

---

## Churn por variables categóricas

Se analizaron variables como:

- género
- tipo de contrato
- método de pago
- servicios contratados

Los resultados muestran que el **tipo de contrato es uno de los factores más influyentes**.

---

## Churn por variables numéricas

Se analizaron variables como:

- antigüedad del cliente
- gasto mensual
- gasto total
- cuentas diarias

Los gráficos utilizados fueron:

- **boxplot**
- **histogramas**

---

## Análisis de correlación

Se calculó una **matriz de correlación** entre variables numéricas y se visualizó con un **heatmap**.

Esto permitió identificar relaciones importantes entre variables como:

- gasto total
- antigüedad del cliente
- cantidad de servicios

---

# 🔍 Principales insights

El análisis permitió identificar varios patrones relevantes:

- Los clientes con **menor antigüedad** presentan mayor churn.
- Los contratos **month-to-month** tienen mayor evasión.
- Los clientes con **mayor gasto mensual** tienden a cancelar más.
- El método de pago **Electronic Check** está asociado a mayor churn.
- Los contratos de **largo plazo** presentan mayor retención.

---

# 💡 Recomendaciones estratégicas

A partir de los resultados del análisis se proponen las siguientes estrategias:

### Incentivar contratos de largo plazo
Ofrecer descuentos o beneficios a clientes que elijan contratos anuales.

### Mejorar la retención de nuevos clientes
Implementar estrategias de fidelización durante los primeros meses.

### Analizar planes de alto costo
Revisar la relación entre precio y percepción de valor.

### Promover pagos automáticos
Incentivar métodos de pago automáticos para mejorar la permanencia.

---

# ▶️ Cómo ejecutar el proyecto

1️⃣ Clonar el repositorio

```bash
git clone https://github.com/tu-usuario/TelecomX_LATAM.git
````

2️⃣ Instalar dependencias

```bash
pip install pandas numpy matplotlib seaborn
```

3️⃣ Abrir el notebook

```
TelecomX_LATAM.ipynb
```

Puede ejecutarse en:

* **Jupyter Notebook**
* **Google Colab**

---

# 👩‍💻 Autor

**Magalí Aldana Suárez**

Estudiante de **Licenciatura en Sistemas**

Interesada en **Data Science, análisis de datos y tecnología**.
