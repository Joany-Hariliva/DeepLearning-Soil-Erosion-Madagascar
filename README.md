# 🤖 Deep Learning for Soil Erosion Modeling
**Predicting Landslide (Lavaka) Susceptibility using Artificial Neural Networks & Multi-source Data Fusion**

## 📊 Performance du Modèle ANN
Avant l'application terrain, le modèle a été rigoureusement validé sur un inventaire de plus de **4 000 points**. Le réseau de neurones (ANN) démontre une forte capacité de généralisation.

* **AUC (Area Under Curve) :** 0.8853
* **Feature Engineering :** Fusion de données Sentinel-2 (NDVI), SRTM (Topographie) et WorldClim.

![Courbe de Performance ROC](./Courbes/04_Courbe_ROC.png)

*L'analyse complète des métriques (Matrice de confusion, Calibration) est disponible dans le dossier [Courbes/](./Courbes).*

---

## 🌍 Application : Cartographie Prédictive
Une fois validé, le modèle a été déployé pour générer une carte de susceptibilité à haute résolution du Bassin Versant de l'Alaotra. C'est l'étape de **déploiement du modèle** sur des données réelles non vues.

![CARTE DE LA SUSCEPTIBILITÉ](./Cartes/Cartes.jpg)

*Les résultats localisent les zones prioritaires pour les interventions de conservation. Livrables SIG disponibles dans le dossier [Cartes/](./Cartes).*

---

## 📂 Structure du Repository
* `Code.ipynb` : Pipeline complet (Preprocessing, Training PyTorch, Evaluation).
* `/Courbes` : Visualisations Data Science (ROC, Importance des variables).
* `/Cartes` : Résultats de l'inférence spatiale (Cartographie finale).
