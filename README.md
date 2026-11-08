# Pronóstico de violencia intrafamiliar en Colombia

App de Streamlit que pronostica la cantidad mensual de casos denunciados de violencia
intrafamiliar por departamento, con un modelo de regresión lineal entrenado sobre el
dataset de la Policía Nacional (Kaggle: *domestic-violence-in-colombia*, 2010–2021).

## Estructura

| Archivo | Función |
|---|---|
| `app.py` | Interfaz: entradas en la barra lateral y pestañas de pronóstico, exploración y modelo |
| `prediccion.py` | Carga el modelo y construye las variables igual que en el notebook |
| `modelo_violencia.pkl` | Modelo, scaler y columnas exportados desde el notebook |
| `historial_mensual.csv` | Casos por departamento y mes, necesarios para calcular los rezagos |
| `.streamlit/config.toml` | Colores de la app |

## Ejecutar en local

```bash
pip install -r requirements.txt
streamlit run app.py
```
