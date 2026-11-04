<div align="center">

# Manuel RAMANITRA

## Ingénieur Data & BI · Lyon
**Je fiabilise les flux de données et je les transforme en tableaux de bord utiles à la décision.**

🔄 ~100 flux critiques supervisés au quotidien (~60 000 exécutions/mois) • 🧱 Databricks & Snowflake (projets perso) • 📊 Power BI

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/manuel-ramanitra)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:manu.rmt@yahoo.com)

![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoft-sql-server&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle_SQL-F80000?style=flat-square&logo=oracle&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=microsoft-power-bi&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![Pentaho](https://img.shields.io/badge/Pentaho_PDI-3E8E41?style=flat-square)
</div>

---

<!--
## 🎯 Ce que je recherche
Un poste d'**Ingénieur Data / BI** ou de **Business Analyst Data**, à l'interface entre les équipes métier et la technique. Basé à Lyon. [À COMPLÉTER : disponibilité / mobilité]
-->

| 🧭 Aller à | |
| :--- | :--- |
| [💼 Expérience en production](#-expérience-en-production--clariane) | [🛠️ Projets Data Engineering](#️-projets-data-engineering-projets-personnels) |
| [📊 Projets Power BI](#-projets-power-bi-projets-personnels) | [🏅 Badges & formation continue](#-badges--formation-continue) |

---

## 🎯 Ce que j'apporte à une équipe

| Votre besoin | Ce que je fais concrètement |
| :--- | :--- |
| **Des chiffres fiables** | Contrôles de qualité automatiques : les données erronées sont détectées, isolées et tracées avant d'arriver dans les rapports. |
| **Des flux qui ne s'arrêtent pas** | Supervision N2/N3 de flux critiques en production, analyse des incidents jusqu'à la cause racine. |
| **Des tableaux de bord clairs** | Dashboards Power BI pensés pour les utilisateurs métier, pas seulement pour les techniciens. |
| **Un dialogue fluide avec le métier** | Cadrage du besoin, ateliers métier, cahiers des charges, spécifications techniques, recette. |
| **Des données bien rangées** | Architecture en couches (brutes → nettoyées → prêtes à analyser), historisation, traçabilité. |

---

# 💼 Expérience en production : Clariane
*Ingénieur Data · BIAL-X en mission chez Clariane · depuis décembre 2024*

Des applications santé, finance, RH et relation client s'échangent chaque jour des données critiques. Un flux en panne ou erroné peut bloquer un service ou fausser un chiffre.

- **Supervision & MCO (N2/N3)** : ~100 flux quotidiens, ~60 000 exécutions/mois, continuité de service.
- **Industrialisation ETL** : conception, test, optimisation et déploiement de flux **Pentaho PDI** (santé, finance, RH, CRM) sur SQL Server, PostgreSQL et Oracle ; livraisons via Git.
- **Fiabilisation** : refonte de la gestion des erreurs, indicateurs de qualité pour les équipes métier, spécifications techniques.
- **Sécurité & traçabilité** : chiffrement, logs, traçabilité des données en erreur.
- **Recette** : recette des flux Pentaho et des rapports Power BI (avec gestion des versions).
- **Flux RH** : transfert automatique des bulletins de paie vers un coffre-fort numérique, flux comptables RH vers l'ERP finance, requêtes SQL d'automatisation des données RH.
- **SQL Oracle** : refactoring de requêtesde suivi des flux Pentaho.

**Résultat** : des flux critiques qui tournent chaque jour, des données de meilleure qualité pour les métiers, des requêtes plus faciles à maintenir. ex. délai de résolution d'incident divisé par deux.

**Stack** : Pentaho PDI • SQL Server • Oracle SQL/PL-SQL • PostgreSQL • Git • REST API (Postman) • WinSCP • ITCare

---

# 🛠️ Projets Data Engineering (projets personnels)
> Projets personnels réalisés en autoformation pour approfondir les plateformes Lakehouse et dbt, avec des jeux de données publics/simulés. Logique commune : architecture **Médaillon** (Bronze → Silver → Gold).

| Projet | Ce qu'il démontre | Stack | Code |
| :--- | :--- | :--- | :--- |
| 🏦 **Banque** | Qualité, quarantaine, SCD1/SCD2, dashboard | Databricks • DLT • PySpark | [Code](https://github.com/Manu-RMT/databricks_bank) |
| ✈️ **Flights** | Ingestion incrémentale, CDC, modèle en étoile | Databricks • DLT • Auto Loader | [Code](https://github.com/Manu-RMT/databricks_flights) |
| ❄️ **Airbnb** | dbt de niveau production, snapshots SCD2, tests | Snowflake • dbt • AWS | [Code](https://github.com/Manu-RMT/DBT_Cloud_Snowflake_AWS_AIRBNB) |
| 🛒 **E-commerce** | Pipeline complet jusqu'au dashboard | Databricks • PySpark • SQL | [Code](https://github.com/Manu-RMT/databricks-ecommerce) |
| 🎬 **TMDB** | Fonctions PySpark réutilisables, dashboard | Databricks • PySpark | [Code](https://github.com/Manu-RMT/databricks-movies-analytics) |

> 🔧 **En cours** : orchestration Airflow (Astronomer Cosmos) et CI/CD GitHub Actions sur un projet dbt + Databricks.
## 🏦 Banque : clients et transactions
**Problème** : des données clients, comptes et transactions de qualité inégale ; les erreurs doivent être repérées avant d'atteindre les rapports.
**Réalisation** : pipeline Landing → Bronze → Silver → Gold en Delta Live Tables, règles de qualité (Expectations), **quarantaine** des lignes invalides, **SCD1** (clients) et **SCD2** (transactions), tables Gold pour la BI.
**Résultat** : pipeline sans intervention manuelle, données invalides isolées plutôt que supprimées, dashboard (indicateurs clés, segmentation, suivi des risques).

| | |
| :---: | :---: |
| <img width="400" src="https://github.com/user-attachments/assets/9c9e0ca7-2607-4f11-831e-0fdcf16259ff" alt="Dashboard bancaire - vue 1" /> | <img width="400" src="https://github.com/user-attachments/assets/0d7b7293-333b-4ebf-a5d5-df564901a4bc" alt="Dashboard bancaire - vue 2" /> |

<details>
<summary>🔧 Détails techniques</summary>

- Auto Loader en streaming ; règles de validité technique (`VALID_RULES`) séparées des filtres métier (`BUSINESS_FILTERS`)
- Transformations centralisées dans `clean_df()` pour éviter les écarts entre tables
- Table matérialisée intermédiaire pour maîtriser l'ordre d'évaluation des règles DLT
- Lignes rejetées conservées dans une table dédiée pour analyse
</details>

🔗 [Voir le code](https://github.com/Manu-RMT/databricks_bank)

---

## ✈️ Flights : vols et réservations
**Problème** : des CSV bruts (vols, aéroports, clients, réservations) non exploitables tels quels.
**Réalisation** : pipeline Databricks en 3 couches (DLT) : ingestion incrémentale avec Auto Loader, contrôles qualité, CDC, puis modèle en étoile (dimensions Customers/Airports, faits Flights/Bookings). Code modulaire et réutilisable.
**Résultat** : données propres, historisées, pipeline relançable sans intervention manuelle.

<img width="500" src="https://github.com/user-attachments/assets/2a514672-8cee-48cb-bd11-0cf47c37dc00" alt="Architecture du pipeline Flights" />

🔗 [Voir le code](https://github.com/Manu-RMT/databricks_flights)

---

## ❄️ Airbnb : entrepôt dbt + Snowflake
**Problème** : alimenter un entrepôt fiable et maintenable à partir de données AWS.
**Réalisation** : chargement AWS → Snowflake, couches staging / intermediate / marts, modèles éphémères, **snapshots SCD2**, tests natifs dbt (`unique`, `not_null`, `relationships`, `accepted_values`) et dbt-expectations.
**Résultat** : qualité vérifiée à chaque exécution, historique conservé, marts prêts pour l'analyse.

🔗 [Voir le code](https://github.com/Manu-RMT/DBT_Cloud_Snowflake_AWS_AIRBNB)

---

## 🛒 E-commerce et 🎬 TMDB
- **E-commerce** : pipeline Bronze → Silver → Gold, faits et dimensions en étoile, dashboard Databricks SQL. [Code](https://github.com/Manu-RMT/databricks-ecommerce)
- **TMDB** : transformations PySpark standardisées, couches Silver/Gold, dashboard SQL interactif. [Code](https://github.com/Manu-RMT/databricks-movies-analytics)

<details>
<summary>🖼️ Captures d'écran</summary>

| | |
| :---: | :---: |
| <img width="400" src="https://github.com/user-attachments/assets/fe470c7d-c0ae-496b-b7ca-8005b9a1855d" alt="E-commerce 1" /> | <img width="400" src="https://github.com/user-attachments/assets/1110392e-c743-4145-bce7-e5405f6db35f" alt="E-commerce 2" /> |
| <img width="400" src="https://github.com/user-attachments/assets/573559a0-bd32-4409-84c8-1c9e366958c9" alt="E-commerce 3" /> | <img width="400" src="https://github.com/user-attachments/assets/1af70399-b010-437b-a965-4f514cc73b92" alt="E-commerce 4" /> |
| <img width="400" src="https://github.com/user-attachments/assets/91476ba7-a83f-41da-91b5-425de400ecf5" alt="TMDB 1" /> | <img width="400" src="https://github.com/user-attachments/assets/9076cddf-a476-4b25-a19f-430efa117f1c" alt="TMDB 2" /> |
</details>

---

# 📊 Projets Power BI (projets personnels)
De la préparation des données au modèle, aux indicateurs **DAX** et à la mise en forme pour le métier.

| Rapport | Objectif | Indicateurs clés | Code |
| :--- | :--- | :--- | :--- |
| 📈 **Suivi de projet** | Suivi de santé d'un projet | Avancement planning, Coût estimé à terminaison, Tâche critique | [Code](https://github.com/Manu-RMT/01_PBI_Gestion_Projet) |
| 🛒 **Hypermarché** | Pilotage commercial | CA Global, Profits, Rentabilité par magasin | [Code](https://github.com/Manu-RMT/Hypermarche-Power-BI) |
| 👥 **Ressources humaines** | Effectifs, promotions, retraites, mobilité | NB effectif droit promotion, Répartition H/F dans les services, Ancienneté  | [Code](https://github.com/Manu-RMT/RH_Power_BI) |

| | | |
| :---: | :---: | :---: |
| <img width="300" alt="Rapport Suivi de projet" src="https://github.com/user-attachments/assets/ed13e4ab-f834-4391-8115-521b2f7bf659" /> | <img width="300" src="https://github.com/user-attachments/assets/3babb931-53d3-4817-9512-a68d3e406c80" alt="Rapport Hypermarché" /> | <img width="300" src="https://github.com/user-attachments/assets/3c0820e5-9ab7-453f-ac8a-0f851fd00143" alt="Rapport RH" /> |

---

# 🏅 Badges & formation continue
- **Snowflake Hands-On Essentials** : badges Data Warehousing, Data Engineering, Data Lake, Data Sharing, Data Application Builders.
- **IA agentique** (en cours, autoformation) : LLM, RAG, agents sur plateformes data.

# 🧭 Parcours

| Période | Poste | Entreprise |
| :--- | :--- | :--- |
| Déc. 2024 – aujourd'hui | **Ingénieur Data** : flux en production | Clariane (via BIAL-X) |
| Sept. 2023 – sept. 2024 | Développeur BI & Informatique Projet (alternance) | Framatome |
| Mai – août 2023 | Développeur BI & Power Platform (stage) | Handicap International |
| Mai – août 2022 | Développeur informatique (stage) | Néatemys |
| Nov. 2019 – août 2021 | Analyste développeur web & logistique | Solulog |

**🎓 Formation** : 
> - M2 Business Intelligence & Analytics (Lyon 2)
> - M1 Informatique (Lyon 2)
> - L3 MIASHS-IDS (Lyon 2)
> - DUT Informatique (IUT de Reims)
  
**🌍 Langues** :
   > - français (natif)
   > - anglais B2
   > - espagnol B1

<details>
<summary>🛠️ <b>Stack complète, par niveau d'expérience</b></summary>

| Niveau | Outils |
| :--- | :--- |
| **En production / emploi** | Pentaho PDI, SQL Server, Oracle SQL & PL/SQL, PostgreSQL, Power BI, Power Query, Git, REST API (Postman) |
| **Stages, alternance, postes précédents** | SSIS, Power Apps, Power Automate, VBA, SAP/Primavera P6 (extraction), Django, PHP |
| **Projets perso & autoformation** | Databricks, PySpark, Delta Live Tables, Snowflake, dbt, Docker, Python (Pandas) |
| **Notions** | C# (formation DUT) |

**Méthodes** : Agile/Scrum, Jira, cycle en V, modélisation dimensionnelle (étoile, SCD 1/2), cahiers des charges.
</details>

---
💡 **Ma conviction** : une bonne donnée est fiable, comprise et utilisée. J'aime relier la technique et le métier pour que les pipelines et les dashboards servent vraiment les équipes.

📬 [LinkedIn](https://www.linkedin.com/in/manuel-ramanitra) • [manu.rmt@yahoo.com](mailto:manu.rmt@yahoo.com)
