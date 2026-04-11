## Contexte du Projet

Avec la généralisation du télétravail et l'omniprésence des réseaux sociaux, les employés passent une partie significative de leur journée connectés à différentes plateformes numériques. Si ces outils peuvent parfois favoriser la communication et la créativité, ils peuvent aussi devenir une source de distraction impactant directement la performance au travail.

Cette étude vise à identifier les facteurs de baisse de performance des salariés en analysant leur productivité réelle à partir de leurs habitudes de travail, leur temps consacré aux réseaux sociaux, leur mode de vie et leur type de métier.

## Problématique

### Problématique Métier

Comment prédire le niveau de productivité des employés à partir de leurs habitudes et leur style de vie ?

### Problématique ML (Non Supervisé)

L'analyse des clusters d'employés montre que la productivité réelle, la perception de productivité et la satisfaction au travail varient fortement entre les groupes, contrairement aux autres variables. Cela soulève la question : comment la satisfaction et la perception de productivité influencent-elles la productivité réelle ?

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
