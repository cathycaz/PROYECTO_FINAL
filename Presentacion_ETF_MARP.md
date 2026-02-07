---
marp: true
title: Flujo de Trabajo - Prediccion de ETFs
paginate: true
size: 16:9
---

<style>
  * {
    margin: 0;
    padding: 0;
  }
  
  section {
    padding: 25px 40px 35px 40px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
    background: #000000;
    color: #ffffff;
  }
  
  section > h1,
  section > h2 {
    width: 100%;
    text-align: left;
    color: #ffffff;
  }
  
  section h1 {
    font-size: 2em;
    margin-bottom: 3px;
    margin-top: 0px;
    word-wrap: break-word;
    color: #00d4ff;
  }
  
  section h2 {
    font-size: 1.4em;
    margin-bottom: 3px;
    word-wrap: break-word;
    color: #ffffff;
  }
  
  section ul {
    font-size: 0.9em;
    margin-left: 15px;
    margin-bottom: 8px;
    width: 100%;
    text-align: left;
    color: #ffffff;
  }
  
  section li {
    margin-bottom: 4px;
    line-height: 1.3;
    color: #e0e0e0;
  }
  
  img {
    max-width: 90%;
    max-height: 60vh;
    width: auto;
    height: auto;
    margin: 50px auto 0 auto;
    object-fit: contain;
  }
  
  .autores {
    position: absolute;
    bottom: 20px;
    right: 30px;
    text-align: right;
    font-size: 0.75em;
    color: #b0b0b0;
    line-height: 1.4;
  }
</style>

# CJC FINANZAS
## Predicción de ETFs

- Objetivo: Estimar precios a 5 días
- Público: No técnico

![Logo](logo.jpeg)

<div class="autores">
<strong>Autores:</strong><br>
Catherine Cazorla<br>
Jesús Jiménez<br>
Carlos Mairena
</div>

---

# Flujo de Trabajo

![Mapa mental](assets/mapa_mental.svg)

---

# Fuentes de Datos y Variables

![Imagen](assets/fuentes.png) 

---

# Integración del Dataset

- Unir ETFs + Variables Exógenas
- Calendario y Trazabilidad de Fechas

![Imagen](assets/linea_tiempo.png)

---

# Causas de Datos Faltantes

![Imagen](assets/faltantes.png)

---

# Análisis Univariante

![ETFs](assets/etfs_univariante.png)

---

# Análisis de Outliers

![Outliers ETFs](assets/outliers_etfs.png)

---

# Métodos de Imputación

- Forward Fill - Backward Fill

![Imagen](assets/imputacion.png)

---

# Preparación de Datos Para Modelos

![Imagen](assets/datos.png)

---

# Modelado (LSTM)

- Modelos directos por dia
- Datos recientes (5 anos)

![Arquitectura simple](assets/arquitectura_lstm.svg)

---

# Evaluacion y validacion

- MAE, RMSE, R², MAPE
- Walk-forward y validacion cruzada

![Comparativa metricas](assets/metricas_etf.svg)

---

# Entrega de predicciones

- 5 dias laborales
- Resumen por ETF

![Tablero de resultados](assets/tablero_resultados.svg)
