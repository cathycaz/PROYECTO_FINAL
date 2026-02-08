---
marp: true
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
    max-width: 95%;
    max-height: 75vh;
    width: auto;
    height: auto;
    margin: 50px auto 0 auto;
    object-fit: contain;
  }
  
  img.large {
    max-width: 95%;
    max-height: 70vh;
    margin: 20px auto 0 auto;
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

- Objetivo: Estimar precios a 5 días
- Público: No técnico

<div class="autores">
<strong>Autores:</strong><br>
Catherine Cazorla<br>
Jesús Jiménez<br>
Carlos Mairena
</div>

![Logo](logo.jpeg)

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
- Modelos Directos por Día
- Datos Recientes (5 años)

<img src="assets/mapa_mental_lstm.svg" class="large" alt="Mapa mental LSTM">

---

# Evaluación y Validación

- Un modelo LSTM por día (horizonte 1 a 5)
- Métricas Obtenidas

<img src="assets/metricas_modelos_directos.svg" class="large" alt="Métricas modelos directos">

---

# Validación Walk-Forward

Método de comprobación temporal que simula predicciones en tiempo real. El modelo se entrena con datos históricos y se valida en seguimiento incremental. Cada paso "camina hacia adelante" incorporando nuevos datos y re-entrenando

<img src="assets/metricas_walk_forward.svg" class="large" alt="Métricas Walk-Forward">

---

# Entrega de predicciones

- 5 dias laborales
- Resumen por ETF

![Tablero de resultados](assets/tablero_resultados.svg)
