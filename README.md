# Analyse de la Productivité des Employés : Impact des Réseaux Sociaux et du Style de Vie

## Contexte du Projet

Avec la généralisation du télétravail et l'omniprésence des réseaux sociaux, les employés passent une partie significative de leur journée connectés à différentes plateformes numériques. Si ces outils peuvent parfois favoriser la communication et la créativité, ils peuvent aussi devenir une source de distraction impactant directement la performance au travail.

## Problématique

### Problématique Métier

Comment prédire le niveau de productivité des employés à partir de leurs habitudes et leur style de vie ?

### Objectifs métier
Cette étude vise à identifier les facteurs de baisse de performance des salariés en analysant leur productivité réelle à partir de leurs habitudes de travail, leur temps consacré aux réseaux sociaux, leur mode de vie et leur type de métier. Grace à elle, les entreprises pourront adapter leur management pour optimiser les facteurs de performance de leurs salariés en ciblant les profils spécifiques et en identifiant les leviers de motivation. Ses résultats aideront surtout les ressources humaines et la direction, à proposer des solutions, faire de la prévention pour la santé mentale et améliorer la cohésion et les conditions de travail.

## Dataset : social_media_vs_productivity

Le dataset comprend 18 variables :

**Variables démographiques et professionnelles**

- `age` : Âge des salariés
- `gender` : Genre
- `job_type` : Type de métier
- `work_hours_per_day` : Temps de travail quotidien

**Variables réseaux sociaux**

- `daily_social_media_time` : Temps quotidien sur les réseaux sociaux
- `social_platform_preference` : Réseau social préféré
- `number_of_notifications` : Notifications reçues par jour
- `weekly_offline_hours` : Heures déconnectées par semaine

**Variables productivité**

- `perceived_productivity_score` : Sentiment de productivité
- `actual_productivity_score` : **Productivité réelle (variable cible)**
- `job_satisfaction_score` : Satisfaction au travail
- `stress_level` : Niveau de stress
- `days_feeling_burnout_per_month` : Jours de burnout par mois

**Variables style de vie**

- `sleep_hours` : Temps de sommeil quotidien
- `screen_time_before_sleep` : Temps d'écran avant de dormir
- `breaks_during_work` : Nombre de pauses au travail
- `uses_focus_apps` : Utilisation d'apps de concentration
- `coffee_consumption_per_day` : Cafés consommés par jour

### Méthodologie

EDA : Analyse statistique, visualisations, corrélations, prise de décisions

Preprocessing : Traitement des valeurs manquantes, encodage, standardisation

Modélisation : Splitting, Entraînement, Test, optimisation, comparaison

Évaluation : Métriques (RMSE, MAE, R², MSE), feature importance

## Modèles Utilisés

### Modèles Supervisés (Régression)

**Random Forest Regressor**

- Algorithme d'ensemble basé sur des arbres de décision
- Excellente capacité à capturer les relations non-linéaires
- Robuste face aux outliers

**ExtraTrees Regressor**

- Algorithme basé sur des arbres de décision
- Capture efficacement les interactions complexes entre les variables
- Moins sensible au surapprentissage grâce à la sélection aléatoire des caractéristiques

**Gradient Boost Regressor**

- Combine plusieurs modèles faibles pour créer un modèle robuste
- Performant pour les données avec des relations non-linéaires
- Peut nécessiter un réglage précis des hyperparamètres pour éviter le surapprentissage

**Classification supervisée : Support Vector Classifier (SVC)**

- Algorithme de classification efficace pour les données de petite taille.
- Utilise des marges maximales pour séparer les classes.

### Modèle Non Supervisé (Classification)

**KMeans Clustering**

- Segmentation des employés en groupes homogènes
- Identification de profils types selon leurs habitudes

### Réduction de dimension

**PCA**

- Réduit la dimensionnalité des données tout en conservant l'essentiel de l'information
- Utile pour visualiser les données et améliorer les performances des modèles

### Conclusion

L'étude révèle que les employés les plus satisfaits sont également ceux qui se perçoivent comme les plus productifs et qui présentent la productivité réelle la plus élevée. Les autres variables (temps sur réseaux sociaux, notifications, heures de travail) n'apportent pas de différence significative entre les groupes.

Pour améliorer la performance globale, il est crucial de se concentrer sur la satisfaction et la perception de productivité. Cela suggère que les actions visant à augmenter le bien-être et la satisfaction des employés peuvent directement accroître leur productivité réelle.

#### Recommandations

- Favoriser l'inclusion pour renforcer le sentiment d'appartenance des salariés à l'entreprise.
- Promouvoir des ateliers de prévention du mal-être, du stress et de suivi de la santé mentale des salariés.
- Mettre en avant une politique et un environnement visant à renforcer le sens de la contribution des salariés (augmentations, prise de responsabilités, valorisation du travail, formations).

#### Limitations

- Les données peuvent contenir des biais liés à l'auto-déclaration des employés.
- Les modèles utilisés ne capturent pas nécessairement toutes les interactions complexes entre les variables.

#### Travaux futurs

- Intégrer des données supplémentaires, comme les performances à long terme des employés.
- Étudier l'impact des politiques de télétravail sur la productivité.
