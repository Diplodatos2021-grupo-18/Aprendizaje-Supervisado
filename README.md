# Aprendizaje-Supervisado

Entrega de la materia aprendizaje supervisado.

## Análisis Exploratorio:
En el archivo data-analysis realizamos un análisis exploratorio del dataset, en el cual observamos las variables y sus relaciones.

## Transformaciones:
Transformamos las variables numéricas 'Age', 'Annual Income' en discretas, con KbinsDiscretizer, utilizando 5 categorías y estrategia 'quantile'.

Las variables categóricas fueron transformadas utilizando 'OneHotEncoder'.

## Modelos:
Evaluamos los modelos: SVM, Knn, Random Forest, Boosting. Utilizamos GridsearchCV y RandomizedSearchCV para la búsqueda de hiperparametros, utilizando Cross Validation, la métrica a optimizar elegida fue f1_Score.

Evaluamos los modelos con la totalidad de datos, comparando los resultados sobre el conjunto de entrenamiento, sin apartar un conjunto de test, ya que consideramos que por la cantidad de datos, era conveniente utilizarlos en su totalidad para entrenar los modelos y luego observar los resultados sobre el conjunto de la competencia. 

## Conclusiones:

Observando la matriz de confusión y Classification Report de los modelos evaluados, los modelos obtuvieron valores bajos en la métrica 'Recall' de la clase positiva, es decir predijeron como negativas etiquetas que en realidad eran positivas. 

Los modelos que lograron superar el Baseline fueron RandomForest y Boosting, siendo RandomForest el de mejores resultados en la competencia Kaggle.


