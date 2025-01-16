# But du Projet:

Création de modèles prédictifs basés sur les données de l'Indice de volume des ventes pour l'ensemble du commerce en France.

# Les méthodes de prévisions utilisées:
   
Pour élaborer un modèle prédictif fiable, nous parcourons trois méthodes et comparons leurs puissances de prédiction :**

      → Méthodes de décomposition
      → Le lissage : Holt, Holt-Winters additive et Holt-Winters multiplicative
      → Méthode de Box-Jenkins.

### 1 Méthode de décomposition**

      1.1 Choix de la méthode . . . . . . . . . . . . . . . . . . . . . . 
      1.2 Méthode de decomposition : Modèle multiplicatif . . . . . .     
      1.2.1 Calcul de la tendance par filtrage par moyenne mobile
      1.2.2 Calcul des coefficients saisonniers . . . . . . . . . . . .
      1.2.3 Série sans variations saisonnières : CVS . . . . . . . .
      
### 2 Le lissage**

      2.1 Méthode de Holt . . . . . . . . . . . .
      2.2 Méthode de Holt-Winters additive . .
      2.3 Méthode de Holt-Winters multiplicatif
      2.4 Meilleure méthode . . . . . . . . . . .
      2.5 Prévision . . . . . . . . . . . . . . . .

### 3 Méthode de Box-Jenkins**

      3.1 Analyse des données . . . . . . . . . . . . . . . . . .
      3.2 Identification du modèle . . . . . . . . . . . . . . . .
      3.3 Apprendre un modèle AR(13) . . . . . . . . . . . . .
      3.4 Validation du modèle . . . . . . . . . . . . . . . . . .
      3.4.1 Significativités des coefficients . . . . . . . . .
      3.4.2 Les Résidus sont-ils des bruits blancs ? . . . .
      3.5 Prévisions . . . . . . . . . . . . . . . . . . . . . . . .
      3.6 Analyse de la capacité prédictive du modèle : MAPE


  # Conclusion :
                          
En comparant les deux méthodes de modélisation, le **lissage** et la méthode de **Box-Jenkins**, nous observons des performances différentes en termes de précision des prédictions. Dans le cas du **lissage**, nous avons utilisé plusieurs variantes de la méthode de **Holt**, notamment la méthode de **Holt**, **Holt-Winters additive** et **Holt-Winters  multiplicatif**. Les MAPE obtenus sont respectivement de **5.59%, 2.75%, et 2.80%**. Ces valeurs indiquent une précision variable des prédictions, avec une amélioration significative observée avec la méthode de **Holt-Winters additive**, qui a un **MAPE optimal de 2.72%**.
      
En ce sens, on a appliqué ce meuilleur modèle retenu, Holt-Winters additive, pour prédire les données futures (données de 2023) et on a eu un **MAPE de 3.02%**. En revanche, la méthode de **Box-Jenkins** a produit un **MAPE de 2.106838%** sur la prévision des données futures, démontrant une précision supérieure par rapport au Holt-Winters additive.
      
Ainsi, sur la base de la comparaison des **MAPE**, la méthode de **Box-Jenkins** fournir des prédictions plus précises que les méthodes de lissage examinées dans cette analyse.


 # Outils : 
 Le travail a été mené sous le **logiciel R** pour la méthode de Box-Jenkins et sous **Excel** pour les deux autres méthodes.
