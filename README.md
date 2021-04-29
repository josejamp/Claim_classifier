# Claim_classifier

El repositorio contiene:
  - validation_claims.csv: csv con el dataset utilizado para validar el modelo. Contiene tres columnas: *text*, *claim* y *claim_predicted*.
  - Notebook_de_trabajo_Claims.ipynb: notebook comentado y detallado con el estudio inicial de los datos, preprocesado y entrenamiento del modelo, y validación del modelo y estudio de resultados.
  - README.md: este propio fichero *readme*, con información sobre el contenido del repositorio y un pequeño resumen de los experimentos realizado.
 

Todos los experimentos han sido ejecutados en un PC local con las siguientes características:
  - Windows 10
  - CPU: Intel(R) Core(TM) i7-8700K CPU @ 3.70GHz 3.70 GHz
  - 16 Gb RAM
  - GPU: Nvidia GeForce RTX 3080

En el notebook viene detallada el experimento que mejor funcionó, aunque se intenaron otros antes en los que se probaron combinaciones de los siguientes cambios:
  - Número de epochs y número de capas de convolución de la CNN.
  - Se probó a normalizar todos los dígitos del dataset pot el token "<num>".
  - Se entrenó con un número menor de ejemplos de frases no verificables. Se realizaron varias pruebas utilizando en ellas, el 50, 60%, 80% y 90% de los ejemplos negativos disponibles.
  
Estos experimentos resultaban en sobreajustes y en un número de falsos positivos que oscilaba entre el doble y el triple con respecto al experimento que finalmente figura en el notebook.
