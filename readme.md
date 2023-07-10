# Reconnaissance des actions humaines à l'aide de capteurs inertiels

Ce projet vise à réaliser un système de reconnaissance des actions humaines en utilisant des capteurs inertiels. Le code Python fourni effectue plusieurs étapes clés d'un projet d'apprentissage automatique, telles que le chargement des données, l'extraction d'informations pertinentes, la préparation des données, l'entraînement de modèles de classification et l'évaluation des performances.

## Présentation du projet

L'objectif principal du projet est de reconnaître les actions humaines en temps réel à l'aide des capteurs inertiels intégrés dans un smartphone. Les capteurs utilisés sont l'accéléromètre, le gyroscope et le magnétomètre. Les signaux inertiels collectés sont ensuite utilisés en entrée d'un système de reconnaissance d'actions pour identifier l'action exécutée par la personne.

## Étapes du projet

Le projet est découpé en plusieurs étapes, qui sont les suivantes :

1. <span style="color: red;">Chargement</span> et compréhension des données : les données nécessaires au projet sont chargées et explorées afin de comprendre leur structure et leur contenu.
2. <span style="color: red;">Extraction</span> d'informations pertinentes : des attributs pertinents sont extraits des données pour être utilisés dans la phase d'apprentissage.
3. <span style="color: red;">Préparation</span> des données : les données sont préparées en vue de l'apprentissage en effectuant des transformations ou des normalisations.
4. <span style="color: red;">Entraînement</span> d'un modèle de classification : un modèle de classification est entraîné à partir des données préparées pour prédire les actions humaines.
5. <span style="color: red;">Test</span> du modèle : le modèle entraîné est testé sur des données de test pour mesurer et analyser ses performances.
6. <span style="color: red;">Sauvegarde</span> du modèle : une fois toutes les étapes précédentes terminées, le modèle entraîné est sauvegardé pour une utilisation ultérieure.

## Utilisation du code

Le code Python fourni est divisé en plusieurs parties, chacune correspondant à une étape spécifique du projet. Voici un aperçu de ce que fait chaque partie :

1. **data_split(data)** : cette fonction divise les données en ensembles d'entraînement et de test, en fonction d'un ensemble prédéfini. Les ensembles d'entraînement et de test sont ensuite renvoyés sous forme de tableaux pandas.

2. **Préparation des données** : cette partie du code effectue une mise à l'échelle des valeurs des données en utilisant la classe `StandardScaler` de Scikit-Learn. Les données d'entraînement et de test sont transformées en utilisant le même scaler.

3. **Entraînement du modèle KNN** : un modèle de classification K plus proches voisins (KNN) est créé en utilisant la classe `KNeighborsClassifier` de Scikit-Learn. Le modèle est entraîné sur les données d'entraînement et utilisé pour prédire les actions sur les données de test.

4. **Évaluation des performances du modèle KNN** : les performances du modèle KNN sont mesurées en utilisant des métriques telles que le rapport de classification, la matrice de confusion et le score d'exactitude.

5. **Entraînement du modèle Naive Bayes** : un modèle de classification Naive Bayes gaussien est créé en utilisant la classe `GaussianNB` de Scikit-Learn. Le modèle est entraîné sur les données d'entraînement et utilisé pour prédire les actions sur les données de test.

6. **Évaluation des performances du modèle Naive Bayes** : les performances du modèle Naive Bayes sont mesurées et évaluées de la même manière que le modèle KNN.
