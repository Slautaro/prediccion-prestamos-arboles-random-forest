# Predicción de préstamos con árboles de decisión y Random Forest

TP2 de la materia Aprendizaje Automático. Implementación desde cero de un árbol de decisión y un Random Forest (bagging de árboles) para predecir si una solicitud de préstamo es otorgada o rechazada.

## Contenido

- `A_A_2.ipynb`: notebook con la construcción del árbol de decisión, el ensamble de Random Forest y la evaluación de resultados.
- `Préstamo.csv`: dataset con las solicitudes de préstamo (45000 registros) usado para entrenar y evaluar los modelos.
- `TP2.pdf`: consigna del trabajo práctico.
- `Diapositivas.pdf`: diapositivas de la presentación del trabajo.

## Resultado

Sobre el conjunto de prueba, el árbol de decisión individual obtuvo **80.1% de accuracy y F1-score de 0.44**, mientras que el Random Forest (bagging de 10 árboles) obtuvo **78.0% de accuracy y F1-score de 0.31**. En este caso el árbol individual superó al ensamble, probablemente porque el bagging con pocos árboles y bootstrap diluye la señal de un dataset ya bastante desbalanceado.

## Cómo correrlo

```bash
pip install pandas numpy matplotlib
jupyter notebook A_A_2.ipynb
```
