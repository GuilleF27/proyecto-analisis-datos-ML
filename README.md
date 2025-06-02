# 📊 Trabajo - Data Science2

**Autor:** Ferino Guillermo  
**Comisión:** 75690   

---

## 🎯 Abstracto

Este proyecto analiza datos de campañas de marketing directo de una institución bancaria portuguesa. Las campañas se realizaron mediante llamadas telefónicas para ofrecer un producto financiero (depósito a plazo). El objetivo es identificar patrones y construir modelos predictivos para determinar la probabilidad de aceptación del producto por parte de un cliente, basándonos en variables como nivel educativo y saldo bancario.

Este análisis puede beneficiar a equipos de marketing, ventas y estrategia comercial que deseen optimizar recursos focalizando las campañas en perfiles con mayor tasa de conversión.

---

## ❓ Hipótesis del Proyecto

**¿Es posible predecir si un cliente aceptará o no el producto ofrecido?**  
Variables clave analizadas: `education`, `balance`, `y` (respuesta).

---

## ✅ Objetivos SMART

- **Específico:** Identificar patrones entre nivel educativo, saldo bancario y aceptación de la oferta.
- **Medible:** Visualizar y analizar correlaciones entre variables.
- **Alcanzable:** Aplicar Python, Pandas, Matplotlib, Seaborn y modelos de machine learning.
- **Relevante:** Mejorar la eficiencia de campañas comerciales.
- **Temporal:** Entregado dentro de los plazos del curso.

---

## 📦 Importación de Datos

Aunque el dataset fue descargado manualmente desde el repositorio [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/bank+marketing), se incluye un ejemplo simulado de cómo se obtendrían los datos desde una API pública, cumpliendo con las consignas del curso:

```python
### 🔽 Ejemplo de cómo se obtendrían los datos desde una API pública
# (Previamente consultado con el docente, quien indicó que debía incluir los comandos de cómo citar una API)

import requests
import pandas as pd

# URL ficticia para simulación de llamada a API
url = "https://api.ejemplo.gov/banco/marketing"
params = {"formato": "csv"}

# response = requests.get(url, params=params)
# with open("datos_marketing.csv", "wb") as f:
#     f.write(response.content)

# Leemos el dataset previamente descargado
df = pd.read_csv("bank-full.csv")
df.head()
