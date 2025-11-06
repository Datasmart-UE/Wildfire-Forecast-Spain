# Modelo Predictivo de Incendios Forestales en España (2024)

Este proyecto se centra en el análisis y modelado predictivo de incendios forestales en España, utilizando datos satelitales MODIS (NASA) y datos meteorológicos históricos de Meteostat.

Su finalidad es aportar conocimiento y herramientas que permitan mejorar la prevención y respuesta frente a incendios forestales, un fenómeno cada vez más grave debido al cambio climático, y que afecta directamente a la seguridad de la población, al entorno ambiental y a la economía del país.

## Objetivos del Proyecto

- Analizar la distribución y comportamiento de incendios en España durante 2024
- Incorporar información meteorológica para mejorar la precisión predictiva
- Entrenar un modelo de Machine Learning que identifique incendios de alta intensidad
- Generar mapas interactivos de incendios reales y predichos
- Entregar un dossier profesional orientado a tomadores de decisión

## Dataset

| Fuente | Descripción | Formato |
|--------|-------------|---------|
| NASA FIRMS MODIS | Incendios detectados en España durante 2024 | CSV |
| Meteostat | Datos climáticos asociados a cada evento | API |

Variables destacadas:
- Localización: latitud, longitud
- Métricas satelitales: FRP, brillo, confianza
- Temporalidad: fecha, hora
- Clima: temperatura media, precipitación, índice de sequía

## Metodología

1. Limpieza y estructuración del dataset
2. Enriquecimiento con meteorología mediante Meteostat
3. Ingeniería de variables (índice de sequía, temporalidad cíclica)
4. Modelado con Random Forest
5. Evaluación del desempeño
6. Visualizaciones interactivas con Folium

## Resultados

- Precisión global del modelo: **93%**
- Sensibilidad en incendios de alta intensidad: **91%**
- Variables más importantes: brillo, temperatura media, índice de sequía

Se generaron dos mapas interactivos:
- Mapa de incendios reales en España (2024)
- Mapa de intensidad predicha sobre ubicaciones reales

## Requerimientos

pip install -r requirements.txt


## Ejecución

jupyter notebook 01_analisis_incendios.ipynb


## Estructura del repositorio

/
├── data/
│ └── modis_2024_Spain.csv
├── results/
│ ├── mapa_incendios_real.html
│ ├── mapa_predicciones.html
│ ├── confusion_matrix.png
│ ├── feature_importance.png
│ └── 01_analisis_incendios_executed.ipynb
├── src/
│ └── 01_analisis_incendios.ipynb
├── README.md
└── dossier_incendios.pdf 


## Autor

**Andrés Martín Llases**  
Estudiante de Ciencia de Datos — UOC  
Barcelona, España  
andresmllases0@gmail.com  
LinkedIn: https://linkedin.com/in/andres-martin-llases-sorice-77279a195  
GitHub: https://github.com/Datasmart-UE
