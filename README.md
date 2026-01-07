Compte rendu : Prédiction de prix avec RandomForestRegressor
![mon image](https://github.com/user-attachments/assets/08c3e95a-6af9-4d7d-9498-daebb0c47dc3)

1. Objectif du projet
Ce projet a pour objectif de prédire le prix des maisons en fonction de leurs caractéristiques, telles que la superficie, le nombre de chambres, l’emplacement ou l’année de construction. L’idée est de fournir des estimations fiables pour aider les acheteurs et les vendeurs à prendre de meilleures décisions sur le marché immobilier.

2. Jeu de données
Le projet utilise un jeu de données comprenant plusieurs centaines d’exemples, chaque ligne représentant une maison avec ses caractéristiques et son prix. Les colonnes principales incluent :

Superficie (m²)

Nombre de chambres

Localisation

Année de construction

Prix de vente (variable cible)

Le jeu de données a été prétraité pour gérer les valeurs manquantes et convertir les variables catégorielles en valeurs numériques.

3. Algorithme choisi : RandomForestRegressor
Le RandomForestRegressor est un algorithme basé sur les forêts d’arbres décisionnels.

Principe : Il construit plusieurs arbres de décision sur des sous-échantillons du jeu de données, puis combine leurs résultats pour obtenir une estimation finale plus robuste.

Avantages :

Capable de gérer les relations non linéaires entre les caractéristiques et le prix.

Robuste face aux valeurs aberrantes.

Réduit le risque de surapprentissage grâce à la moyenne des arbres.

4. Mise en œuvre
Le modèle a été entraîné sur une partie des données (train set) et testé sur le reste (test set) pour évaluer sa performance. Les hyperparamètres, comme le nombre d’arbres et la profondeur maximale, ont été ajustés pour optimiser la précision.

5. Résultats
Le RandomForestRegressor a permis de prédire les prix avec une bonne précision :

Coefficient de détermination 
𝑅
2
R
2
 : 0,85

L’erreur moyenne (MAE) est faible, ce qui montre que les prédictions sont proches des valeurs réelles.

Un graphique comparant les prix réels et les prix prédits montre que la majorité des prédictions se situent très près de la diagonale idéale, confirmant la performance du modèle.

<img width="870" height="5437" alt="image" src="https://github.com/user-attachments/assets/cf522aa7-0421-4173-ab79-a07bf76ddb40" />


<img width="554" height="448" alt="image" src="https://github.com/user-attachments/assets/9ec75639-3dce-487b-aa23-da53ef77aaff" />

<img width="554" height="448" alt="image" src="https://github.com/user-attachments/assets/8ec8ba86-7e5f-4131-8640-843269ef54b1" />



6. Conclusion
En conclusion, le RandomForestRegressor s’avère être un outil efficace pour la prédiction des prix des maisons. Il fournit des résultats fiables et précis, démontrant l’utilité du machine learning pour la prise de décision dans des situations pratiques, comme le marché immobilier.
