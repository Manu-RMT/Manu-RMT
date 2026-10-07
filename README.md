<div align="center">

# 👨‍💼 Manuel RAMANITRA

## Ingenieur Data & BI : je rends les données fiables, claires et utiles à la décision

**🔄 ~100 flux en production par jour  •  🧱 Plateformes Databricks & Snowflake  •  📊 Tableaux de bord Power BI**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/manuel-ramanitra)

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:manu.rmt@yahoo.com)

![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=microsoft-power-bi&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
</div>

---

## 👋 Qui suis-je ?

Je suis **Ingénieur Data & BI chez Clariane** depuis décembre 2024 (en mission via BIAL-X).

En termes simples : **je construis et je surveille les circuits qui acheminent les données d'une application à l'autre**, puis je les transforme en **tableaux de bord** que les équipes métier utilisent pour décider.

Au quotidien, je suis responsable du bon fonctionnement d'environ **100 flux de données par jour** qui touchent des domaines critiques : **santé, finance, ressources humaines et relation client**.

---

## 🎯 Ce que j'apporte à une équipe

| Votre besoin | Ce que je fais concrètement |
| :--- | :--- |
| **Des chiffres fiables** | Je mets en place des contrôles automatiques : les données erronées sont détectées et isolées avant d'arriver dans les rapports. |
| **Des tableaux de bord clairs** | Je conçois des dashboards **Power BI** lisibles, pensés pour les utilisateurs métier et pas seulement pour les techniciens. |
| **Un service qui ne s'arrête pas** | Je supervise des flux en production et je les fiabilise pour qu'ils tournent chaque jour sans interruption. |
| **L'historique des changements** | Je conserve la trace de ce qui a changé et quand (par exemple une modification de client ou de contrat). |
| **Une communication fluide avec le métier** | Je traduis un besoin métier en solution technique : cahiers des charges, ateliers, méthode Agile (Scrum, Jira). |
| **Des données bien rangées et sécurisées** | Je structure les données en couches (brutes → nettoyées → prêtes à analyser) et j'encadre les accès (gouvernance). |

---

## 🧰 Mes outils, en deux mots

- **Databricks et Snowflake** : les plateformes qui stockent et traitent de gros volumes de données.

- **dbt, PySpark, SQL, Python** : les outils pour nettoyer et transformer les données.

- **Power BI** : l'outil pour transformer les données en tableaux de bord.

- **Git, Docker** : pour travailler proprement en équipe et automatiser.

*Le détail complet est en bas de page.*

---

# 💼 Expérience en production : Clariane

| | |
| :--- | :--- |
| **🅢 Situation** | Au sein de Clariane (mission via BIAL-X), des applications échangent chaque jour des données critiques : **santé, finance, RH et relation client**. Un flux en panne ou erroné peut bloquer un service ou fausser un chiffre. |
| **🅣 Tâche** | Superviser environ **100 flux inter-applicatifs par jour**, garantir leur bon déroulement et corriger rapidement les anomalies. |
| **🅐 Action** | Suivi quotidien des flux en production • analyse des incidents jusqu'à la cause racine • développement et optimisation de requêtes **Oracle SQL / PL/SQL** (dont des requêtes multi-CTE sur des référentiels d'organisation hiérarchiques) • transformations sur **Databricks (PySpark)** et **dbt / Snowflake** • versionnage et déploiement en **GitOps** • travail en **Scrum** avec **Jira** et échanges avec les équipes métier. |
| **🅡 Résultat** | Des flux critiques qui tournent chaque jour de façon fiable, des données de meilleure qualité pour les équipes métier et des requêtes plus lisibles et plus faciles à maintenir. |
<details>
<summary>🔧 Détails techniques</summary>

- **Périmètre :** flux inter-applicatifs santé / finance / RH / client, environnement d'entreprise français

- **Bases & requêtage :** Oracle SQL, PL/SQL, SQL Server, refactoring de requêtes multi-CTE (lisibilité, performance, maintenabilité)

- **Traitement :** Databricks, PySpark, Delta Lake, dbt, Snowflake

- **Pratiques :** GitOps, revue de code, gouvernance des données, rédaction de cahiers des charges, Scrum / Jira

- **Restitution :** Power BI, Power Query, Power Apps / Power Automate
</details>

---

# 🛠️ Projets Data Engineering
> Chaque projet est présenté avec la **méthode STAR** (Situation, Tâche, Action, Résultat), puis le détail technique pour les équipes data.
> Logique commune : **données brutes → données nettoyées → données prêtes à analyser** (architecture « Médaillon » : Bronze, Silver, Gold).

## ✈️ Flights : analyse de vols et de réservations

| | |
| :--- | :--- |
| **🅢 Situation** | Des fichiers CSV bruts de vols, d'aéroports, de clients et de réservations arrivent régulièrement et ne sont pas directement exploitables. |
| **🅣 Tâche** | Construire une plateforme qui charge uniquement les nouvelles données, vérifie leur qualité et les met à disposition pour l'analyse. |
| **🅐 Action** | Pipeline **Databricks** en 3 couches avec **Delta Live Tables** : ingestion incrémentale, contrôles qualité, gestion des changements (CDC), puis modèle en étoile. Code organisé en modules réutilisables. |
| **🅡 Résultat** | Des données propres, historisées et toujours à jour, prêtes pour analyser vols, aéroports, clients et réservations, avec un pipeline relançable sans intervention manuelle. |

<img width="600" height="375" src="https://github.com/user-attachments/assets/2a514672-8cee-48cb-bd11-0cf47c37dc00" />
<details>
<summary>🔧 Détails techniques</summary>

**Architecture**

- **Bronze :** ingestion des CSV (Auto Loader, chargement incrémental) avec journalisation des fichiers traités

- **Silver :** normalisation des types et des formats, contrôles qualité (Expectations), CDC pour suivre créations, modifications et suppressions

- **Gold :** schéma en étoile avec dimensions (Customers, Airports) et faits (Flights, Bookings)

**Choix techniques**

- Delta Live Tables en mode déclaratif : dépendances entre tables gérées par DLT

- Historisation via Delta Lake (versions des tables, retour en arrière possible)

- Code factorisé en modules pour ajouter une table sans dupliquer la logique

**Stack :** Databricks • PySpark • Delta Lake • Delta Live Tables • Auto Loader • SQL
</details>

🔗 [Voir le code sur GitHub](https://github.com/Manu-RMT/databricks_flights)

---

## 🏦 Banque : clients et transactions

| | |
| :--- | :--- |
| **🅢 Situation** | Une plateforme de données bancaires reçoit des données clients, comptes et transactions de qualité inégale. Les erreurs doivent être repérées avant d'atteindre les rapports. |
| **🅣 Tâche** | Mettre en place un pipeline 100 % automatisé qui contrôle, isole les données invalides et conserve l'historique, avec un dashboard de pilotage à la clé. |
| **🅐 Action** | Architecture **Landing → Bronze → Silver → Gold** avec Delta Live Tables. Règles de qualité sur chaque donnée, mise en **quarantaine** des lignes invalides, historisation **SCD1** (clients) et **SCD2** (transactions), tables Gold prêtes pour la BI. |
| **🅡 Résultat** | Un pipeline sans intervention manuelle, des données invalides isolées au lieu de polluer les analyses, et un dashboard bancaire complet : indicateurs clés, segmentation de la clientèle et suivi des risques. |

<img width="600" height="375" alt="Dashboard bancaire - vue 1" src="https://github.com/user-attachments/assets/9c9e0ca7-2607-4f11-831e-0fdcf16259ff" />
<img width="600" height="375" alt="Dashboard bancaire - vue 2" src="https://github.com/user-attachments/assets/0d7b7293-333b-4ebf-a5d5-df564901a4bc" />
<details>
<summary>🔧 Détails techniques</summary>

**Architecture**

- **Landing → Bronze :** ingestion incrémentale (Auto Loader), nettoyage, Expectations, quarantaine

- **Silver :** normalisation, SCD1 sur les clients (on écrase avec la dernière valeur), SCD2 sur les transactions (on garde chaque version), enrichissements

- **Gold :** vues analytiques et agrégations clients / comptes / transactions

**Patterns de conception**

- **Séparation des règles :** règles de validité technique (`VALID_RULES`) distinctes des filtres métier (`BUSINESS_FILTERS`)

- **Transformations centralisées** dans une fonction unique `clean_df()` pour éviter les écarts entre tables

- **Table matérialisée intermédiaire** pour maîtriser l'ordre d'évaluation des règles DLT (`expect`) et éviter des erreurs de séquencement

- **Quarantaine :** les lignes rejetées sont conservées dans une table dédiée pour analyse, au lieu d'être supprimées

- Sources en **streaming**, configuration d'Auto Loader et choix du schéma documentés

**Stack :** Databricks • Delta Live Tables • PySpark • Auto Loader • Databricks SQL
</details>

🔗 [Voir le code sur GitHub](https://github.com/Manu-RMT/databricks_bank)

---

## 🛒 E-commerce : ventes et comportement clients

| | |
| :--- | :--- |
| **🅢 Situation** | Une boutique en ligne produit des données de ventes et de clients dispersées, difficiles à analyser telles quelles. |
| **🅣 Tâche** | Livrer un pipeline de bout en bout, de la donnée brute au dashboard, pour suivre les ventes et les clients. |
| **🅐 Action** | Pipeline **Bronze → Silver → Gold** : normalisation et contrôles qualité, tables de faits et de dimensions, modèle en étoile optimisé pour la BI, dashboard **Databricks SQL**. |
| **🅡 Résultat** | Des données directement exploitables par les équipes métier, avec un dashboard pour suivre l'activité commerciale. |

<img width="600" height="375" src="https://github.com/user-attachments/assets/fe470c7d-c0ae-496b-b7ca-8005b9a1855d" />
<img width="600" height="375" src="https://github.com/user-attachments/assets/1110392e-c743-4145-bce7-e5405f6db35f" />
<img width="600" height="375" src="https://github.com/user-attachments/assets/573559a0-bd32-4409-84c8-1c9e366958c9" />
<img width="600" height="375" src="https://github.com/user-attachments/assets/1af70399-b010-437b-a965-4f514cc73b92" />
<details>
<summary>🔧 Détails techniques</summary>

- **Bronze :** ingestion des données brutes

- **Silver :** normalisation (types, formats, doublons) et contrôles qualité

- **Gold :** tables de **faits** (ventes) et **dimensions** (clients, produits…) en **modèle en étoile**, pensé pour limiter les jointures coûteuses côté BI

- **Restitution :** dashboard Databricks SQL alimenté par les tables Gold

- **Stack :** Databricks • PySpark • Delta Lake • Databricks SQL
</details>

🔗 [Voir le code sur GitHub](https://github.com/Manu-RMT/databricks-ecommerce)

---

## ❄️ Airbnb : entrepôt de données (dbt + Snowflake)

| | |
| :--- | :--- |
| **🅢 Situation** | Des données de type Airbnb (annonces, hôtes, réservations) sont stockées sur AWS et doivent alimenter un entrepôt fiable et maintenable. |
| **🅣 Tâche** | Construire un pipeline **dbt** de niveau production : transformations versionnées, historisées et testées automatiquement. |
| **🅐 Action** | Chargement **AWS → Snowflake**, architecture Médaillon en couches **staging / intermediate / marts**, **snapshots SCD Type 2**, modèles éphémères, stratégie de tests (tests natifs dbt + dbt-expectations). |
| **🅡 Résultat** | Un entrepôt dont la qualité est vérifiée à chaque exécution, avec l'historique des changements conservé et des tables marts prêtes pour l'analyse métier. |
<details>
<summary>🔧 Détails techniques</summary>

- **Ingestion :** sources sur AWS vers Snowflake

- **Staging :** nettoyage et renommage des colonnes sources, sans logique métier

- **Intermediate :** jointures et règles de transformation, via des **modèles éphémères** (pas de table physique inutile)

- **Marts :** tables finales dimensionnelles, prêtes pour la BI

- **SCD Type 2 :** snapshots dbt pour conserver chaque version d'une ligne (dates de début et de fin de validité)

- **Tests :** tests natifs (`unique`, `not_null`, `relationships`, `accepted_values`) et **dbt-expectations** pour des contrôles avancés

- **Stack :** Snowflake • dbt • AWS • SQL • Git
</details>

🔗 [Voir le code sur GitHub](https://github.com/Manu-RMT/DBT_Cloud_Snowflake_AWS_AIRBNB)

---

## 🎬 TMDB : analyse de films

| | |
| :--- | :--- |
| **🅢 Situation** | Des données cinéma (films, notes, genres) sont brutes et hétérogènes. |
| **🅣 Tâche** | Les standardiser et les présenter dans un dashboard interactif. |
| **🅐 Action** | Transformations **PySpark** standardisées, structuration en couches Silver et Gold, dashboard **SQL** interactif. |
| **🅡 Résultat** | Des données structurées et un dashboard permettant d'explorer le catalogue de films. |

<img width="600" height="375" src="https://github.com/user-attachments/assets/91476ba7-a83f-41da-91b5-425de400ecf5" />

<img width="600" height="375" src="https://github.com/user-attachments/assets/9076cddf-a476-4b25-a19f-430efa117f1c" />
<details>
<summary>🔧 Détails techniques</summary>

- Fonctions de transformation PySpark réutilisables et standardisées

- **Silver :** données nettoyées et typées • **Gold :** tables prêtes pour l'analyse

- Dashboard Databricks SQL interactif

- **Stack :** Databricks • PySpark • SQL
</details>

🔗 [Voir le code sur GitHub](https://github.com/Manu-RMT/databricks-movies-analytics)

---

# 📊 Projets Power BI : de la donnée à la décision

Trois tableaux de bord complets : préparation des données, modèle de données, indicateurs (**DAX**) et mise en forme pour les équipes métier.

## 🚗 ShopEasyCar : ventes automobiles
<img width="600" height="375" src="https://github.com/user-attachments/assets/77c0af58-8c89-4e3b-beaa-19ef66412934" />

🔗 [Voir le code sur GitHub](https://github.com/Manu-RMT/ShopEasyCar_Power_BI_-_Python)

---

## 🛒 Hypermarché : pilotage commercial
<img width="600" height="375" src="https://github.com/user-attachments/assets/3babb931-53d3-4817-9512-a68d3e406c80" />

🔗 [Voir le code sur GitHub](https://github.com/Manu-RMT/Hypermarche-Power-BI)

---

## 👥 Ressources humaines : suivi RH
<img width="600" height="375" alt="accueil_pbi_rh" src="https://github.com/user-attachments/assets/f5916b8b-4b21-45db-a0c1-529a49b3349d" />

🔗 [Voir le code sur GitHub](https://github.com/Manu-RMT/RH_Power_BI)

---

# 🧭 Parcours

| Période | Poste | Entreprise |
| :--- | :--- | :--- |
| Déc. 2024 – aujourd'hui | **Ingénieur Data** : flux inter-applicatifs en production | Clariane (via BIAL-X) |
| Sept. 2023 – sept. 2024 | Développeur BI / Ingénieur informatique (alternance) | Framatome |
| Mai – août 2023 | Développeur BI & Power Platform (stage) | Handicap International |
| Mai – août 2022 | Développeur informatique (stage) | Néatemys |
| Nov. 2019 – août 2021 | Analyste développeur / Développeur web | Solulog |

**🎓 Formation :** 
- M2 Business Intelligence & Analytics (Université Lyon 2) 
- M1 Informatique (Lyon 2) 
- L3 MIASHS-IDS (Lyon 2) 
- DUT Informatique (IUT de Reims)

**🌍 Langues :** 
- français (langue maternelle) 
- anglais (B2) 
- espagnol (B1)

---
<details>
<summary>🛠️ <b>Stack technique complète</b> (cliquer pour afficher)</summary>

| **Catégorie** | **Outils & Technologies** |
| :--- | :--- |
| **🧠 Langages & requêtage** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white) ![Oracle SQL](https://img.shields.io/badge/Oracle_SQL-F80000?style=flat-square&logo=oracle&logoColor=white) ![PL/SQL](https://img.shields.io/badge/PL/SQL-F80000?style=flat-square) ![DAX](https://img.shields.io/badge/DAX-F2C811?style=flat-square) ![VBA](https://img.shields.io/badge/VBA-217346?style=flat-square&logo=microsoft-excel&logoColor=white) |
| **☁️ Plateformes Data** | ![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white) ![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white) ![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoft-sql-server&logoColor=white) |
| **🔄 Transformation & intégration** | ![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white) ![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apache-spark&logoColor=white) ![DLT](https://img.shields.io/badge/Delta_Live_Tables-00ADFF?style=flat-square) ![Pentaho](https://img.shields.io/badge/Pentaho-3E8E41?style=flat-square) ![SSIS](https://img.shields.io/badge/SSIS-5C2D91?style=flat-square&logo=microsoft-sql-server&logoColor=white) ![API](https://img.shields.io/badge/Web_API-REST-6DB33F?style=flat-square) |
| **📐 Modélisation & BI** | ![MERISE](https://img.shields.io/badge/MCD/MLD-MERISE-blueviolet?style=flat-square) ![StarSchema](https://img.shields.io/badge/Schéma-Étoile-orange?style=flat-square) ![SCD](https://img.shields.io/badge/SCD-Type_1_%26_2-success?style=flat-square) ![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=microsoft-power-bi&logoColor=black) ![Power Query](https://img.shields.io/badge/Power_Query-F2C811?style=flat-square) |
| **⚙️ Automatisation & DevOps** | ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![GitOps](https://img.shields.io/badge/GitOps-2088FF?style=flat-square) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Power Apps](https://img.shields.io/badge/Power_Apps-742774?style=flat-square&logo=powerapps&logoColor=white) ![Power Automate](https://img.shields.io/badge/Power_Automate-0066FF?style=flat-square&logo=powerautomate&logoColor=white) |
| **📊 Analyse** | ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-013243?style=flat-square) ![NLP](https://img.shields.io/badge/NLP-TextBlob-blueviolet?style=flat-square) |
| **🤝 Méthodes & collaboration** | ![Jira](https://img.shields.io/badge/Jira-0052CC?style=flat-square&logo=jira&logoColor=white) ![Scrum](https://img.shields.io/badge/Scrum-Agile-0052CC?style=flat-square) ![Cycle en V](https://img.shields.io/badge/Cycle_en_V-grey?style=flat-square) ![SharePoint](https://img.shields.io/badge/SharePoint-0078D4?style=flat-square&logo=microsoftsharepoint&logoColor=white) |
</details>

---

💡 **Ma conviction :** une bonne donnée est une donnée fiable, comprise et utilisée. J'aime relier la technique et le métier pour que les pipelines et les tableaux de bord servent vraiment les équipes.

📬 Un échange sur la data ? [LinkedIn](https://linkedin.com/in/manuel-ramanitra) • [manu.rmt@yahoo.com](mailto:manu.rmt@yahoo.com)
 
