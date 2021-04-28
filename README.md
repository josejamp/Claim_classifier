# Claim_classifier
A Claim Bert classifier

El repositorio contiene:
  - validation_claims.csv: csv con el dataset utilizado para validar el modelo. Contiene tres columnas: text, claim y claim_predicted.
  - Notebook_de_trabajo_Claims.ipynb: notebook comentado y detallado con el estudio inicial de los datos, preprocesado y entrenamiento del modelo, y validación del modelo y estudio de resultados.
  - README.md: este propio fichero readme, con información sobre el contenido del repositorio y un pequeño resumen de los experimentos realizado.
 
 
En el notebook viene detallada el experimento que mejor funcionó, aunque se intenaron otros antes en los que se probaron combinaciones de los siguientes cambios:
  - Número de epochs y número de capas de convolución de la CNN.
  - Se probó a normalizar todos los dígitos del dataset pot el token "<num>".
  - Se entrenó con un número menor de ejemplos de frases no verificables.
  
En general, estos experimentos resultaban en sobreajustes y en un número de falsos positivos que oscilaba entre el doble y el triple con respecto al experimento que finalmente figura en el notebook.
