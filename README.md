# PROYECTO FINAL: Predicción de ETFs con Deep Learning

## 🚀 Descripción General
Este proyecto implementa un sistema predictivo de precios para ETFs utilizando modelos de Deep Learning, integrando procesamiento avanzado de datos, visualización interactiva y despliegue web. El objetivo es anticipar movimientos de mercado y facilitar la toma de decisiones financieras mediante inteligencia artificial.

## 🧠 Características Técnicas Destacadas
- **Modelos Secuenciales LSTM** entrenados para predicción multihorizonte (1 a 5 días).
- **Preprocesamiento robusto**: limpieza, imputación y normalización de datos financieros.
- **Visualización avanzada** con gráficos interactivos y dashboards.
- **Despliegue web**: interfaz intuitiva para usuarios finales.
- **Automatización de pipelines** para actualización y reentrenamiento de modelos.

## 🛠️ Habilidades y Tecnologías Utilizadas
- **Python 3.x**
- **TensorFlow / Keras**: Modelado y entrenamiento de redes neuronales profundas.
- **Pandas & NumPy**: Manipulación y análisis eficiente de grandes volúmenes de datos.
- **Scikit-learn**: Preprocesamiento y métricas de evaluación.
- **Streamlit**: Desarrollo de aplicaciones web interactivas.
- **Matplotlib / Plotly**: Visualización de datos y resultados.
- **Jupyter Notebook**: Prototipado y documentación viva.

## 📁 Estructura del Proyecto
- `Home.py`: Interfaz principal de la aplicación.
- `pages/`: Módulos adicionales y páginas secundarias.
- `modelos_directos_recientes/`: Modelos LSTM entrenados para cada horizonte temporal.
- `DataSet_General/`: Dataset limpio y preprocesado.
- `assets/`: Recursos gráficos y multimedia.
- `Modelo_Predictivo.ipynb`: Desarrollo y experimentación del modelo.

## 💡 Innovación y Vanguardismo
- **Predicción multihorizonte**: Modelos independientes para cada día futuro, maximizando precisión.
- **Actualización automática**: Pipeline preparado para ingestión y reentrenamiento continuo.
- **Visualización inmersiva**: Dashboards interactivos y personalizables.
- **Código modular y escalable**: Fácil integración de nuevos modelos y fuentes de datos.

## 📦 Instalación Rápida
1. Clona el repositorio y navega a la carpeta del proyecto.
2. Instala las dependencias:
   ```bash
   pip install -r requirements.txt
   ```
3. Ejecuta la aplicación:
   ```bash
   streamlit run Home.py
   ```

## 🤝 Contribuciones
¡Las contribuciones son bienvenidas! Abre un issue o pull request para sugerir mejoras o nuevas funcionalidades.

## 📝 Licencia
Este proyecto se distribuye bajo la Licencia MIT.
