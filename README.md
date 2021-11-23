# Aprendizaje-Supervisado

Entrega de la materia aprendizaje supervisado.

En el archivo data-analysis realizamos un analisis exploratorio del dataset.

## Transformaciones:
Transformamos las variables numericas 'Age', 'AnnualIncome' en discretas, con KbinsDiscretizer, utilizando 5 categorias y estrategia 'quantile', la cual asigna a cada clase la misma cantidad de puntos.

Las variables categoricas fueron transformadas utilizando 'OneHotEncoder'.

## Modelos:
Evaluamos los modelos: SVM, Knn, Random Forest, Boosting. Utilizamos GridsearchCV y RandomizedSearchCV para la busqueda de hiperparametros, utilizando Cross Validation, la metrica a optimizar elegida fue f1_Score.

## Conclusion:
Los modelos que lograron superar el Baseline fueron RandomForest y Boosting, siendo RandomForest el de mejores resultados en la competencia Kaggle.

