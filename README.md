# Deloitte x The Forage — Data Analytics Virtual Internship
### Daikibo Industrials Case Study

---

## 🇬🇧 ENGLISH VERSION

### Project Overview

This project was completed as part of the **Deloitte Australia Data Analytics Virtual Internship** on The Forage platform. It involved real-world data analysis tasks for a fictional industrial client, **Daikibo Industrials**, a manufacturer operating four factories across the globe.

---

### Task 1 — Machine Downtime Analysis (Tableau Dashboard)

#### Objective
Daikibo's tech team unified telemetry data collected from all 4 factories over the month of **May 2021**. Each factory operates **9 types of machines**, each sending a status message every **10 minutes**. The goal was to answer two key business questions:
1. **In which factory did machines break down the most?**
2. **Which machines broke most often in that location?**

#### Methodology
- Analyzed a unified JSON telemetry dataset using **Tableau Public**
- Built two visualizations: **Downtime Per Factory** and **Downtime Per Machine**
- Machines with an "Unhealthy" status were counted as downtime events

#### Results

| Factory | Total Downtime Events |
|---|---|
| 🔴 **Daikibo Factory Seiko** (Osaka, Japan) | **480** |
| Daikibo Shenzhen (China) | 420 |
| Daikibo Factory Meiyo (Tokyo, Japan) | 110 |
| Daikibo Berlin (Germany) | 20 |

- **Daikibo Factory Seiko** recorded the highest number of machine breakdowns (480 events), making it the most critical site for maintenance intervention.
- Within that factory, the **LaserWelder** was responsible for all 480 downtime events — all other machine types recorded 0 downtime, identifying it as the single point of failure.

---

### Task 2 — Gender Pay Equality Analysis (Excel)

#### Objective
Following internal complaints about gender pay inequality, Daikibo Industrials commissioned a forensic analysis. An algorithm produced an **Equality Score** for each job role at each factory location. The task was to classify these scores and analyze the results.

#### Classification Logic
The equality score was classified using the following rule (implemented as an Excel formula):

| Score (absolute value) | Classification |
|---|---|
| -10 to +10 | ✅ Fair |
| < -10 or > +10 | ⚠️ Unfair |
| < -20 or > +20 | ❌ Highly Discriminative |


#### Results by Factory

| Factory | Fair | Unfair | Highly Discriminative | Average Score |
|---|---|---|---|---|
| Daikibo Berlin | 5 | 3 | 0 | **-5.5** |
| Daikibo Shenzhen | 5 | 2 | 1 | **-10.0** |
| Daikibo Factory Seiko | 4 | 3 | 3 | **-12.6** |
| Daikibo Factory Meiyo | 4 | 4 | 3 | **-14.4** |
| **Overall** | **18** | **12** | **7** | **-11.0** |

#### Key Findings
- **Daikibo Berlin** is the most equitable location, with no "Highly Discriminative" roles and an average score of -5.5.
- **Daikibo Factory Meiyo** (Tokyo) shows the greatest gender pay gap, with the worst average score (-14.4) and 3 highly discriminative roles.
- **7 out of 37 job roles** (19%) across all factories are classified as "Highly Discriminative."
- The pay gap is **consistently negative**, meaning women are systematically underpaid across all locations and seniority levels.
- Senior roles (C-Level, VP, Director) tend to show the most extreme scores, suggesting inequality worsens at higher organizational levels.

---

### Tools Used
- **Tableau Public** — data visualization and dashboard creation
- **Microsoft Excel** — data classification and pivot table analysis

---
---

## 🇫🇷 VERSION FRANÇAISE

### Présentation du projet

Ce projet a été réalisé dans le cadre du **stage virtuel en Data Analytics de Deloitte Australie** sur la plateforme The Forage. Il s'agissait d'analyser des données pour un client industriel fictif, **Daikibo Industrials**, un fabricant exploitant quatre usines à travers le monde.

---

### Tâche 1 — Analyse des pannes machines (Dashboard Tableau)

#### Objectif
L'équipe technique de Daikibo a unifié les données de télémétrie collectées dans les 4 usines durant le mois de **mai 2021**. Chaque usine dispose de **9 types de machines**, envoyant un message de statut toutes les **10 minutes**. L'objectif était de répondre à deux questions clés :
1. **Dans quelle usine les machines sont-elles tombées en panne le plus souvent ?**
2. **Quelles machines ont le plus souvent été en panne dans cette usine ?**

#### Méthodologie
- Analyse d'un jeu de données de télémétrie unifié en JSON via **Tableau Public**
- Création de deux visualisations : **Downtime Per Factory** et **Downtime Per Machine**
- Les machines au statut "Unhealthy" ont été comptabilisées comme des événements de panne

#### Résultats

| Usine | Nombre d'événements de panne |
|---|---|
| 🔴 **Daikibo Factory Seiko** (Osaka, Japon) | **480** |
| Daikibo Shenzhen (Chine) | 420 |
| Daikibo Factory Meiyo (Tokyo, Japon) | 110 |
| Daikibo Berlin (Allemagne) | 20 |

- **Daikibo Factory Seiko** enregistre le plus grand nombre de pannes (480 événements) : c'est le site le plus critique en matière de maintenance.
- Dans cette usine, le **LaserWelder** est responsable de la totalité des 480 pannes — tous les autres types de machines affichent 0 panne, ce qui en fait le seul point de défaillance.

---

### Tâche 2 — Analyse de l'égalité salariale homme/femme (Excel)

#### Objectif
Suite à des plaintes internes relatives à l'inégalité salariale entre les genres, Daikibo Industrials a commandé une analyse forensique. Un algorithme a calculé un **score d'égalité** pour chaque rôle dans chaque usine. La mission consistait à classifier ces scores et à en analyser les résultats.

#### Logique de classification
Le score d'égalité a été classifié selon la règle suivante (implémentée sous forme de formule Excel) :

| Score (valeur absolue) | Classification |
|---|---|
| -10 to +10 | ✅ Équitable |
| < -10 or > +10 | ⚠️ Inéquitable |
| < -20 or > +20 | ❌ Très discriminatoire |


#### Résultats par usine

| Usine | Équitable | Inéquitable | Très discriminatoire | Score moyen |
|---|---|---|---|---|
| Daikibo Berlin | 5 | 3 | 0 | **-5,5** |
| Daikibo Shenzhen | 5 | 2 | 1 | **-10,0** |
| Daikibo Factory Seiko | 4 | 3 | 3 | **-12,6** |
| Daikibo Factory Meiyo | 4 | 4 | 3 | **-14,4** |
| **Total général** | **18** | **12** | **7** | **-11,0** |

#### Conclusions principales
- **Daikibo Berlin** est le site le plus équitable : aucun rôle "très discriminatoire" et un score moyen de -5,5.
- **Daikibo Factory Meiyo** (Tokyo) présente le plus grand écart salarial entre les genres, avec le score moyen le plus bas (-14,4) et 3 rôles très discriminatoires.
- **7 postes sur 37** (soit 19%) dans l'ensemble des usines sont classés "très discriminatoires".
- Le différentiel de rémunération est **systématiquement négatif**, signifiant que les femmes sont sous-payées dans tous les sites et à tous les niveaux hiérarchiques.
- Les postes les plus élevés (C-Level, VP, Directeur) tendent à afficher les scores les plus extrêmes, suggérant que les inégalités s'aggravent avec le niveau hiérarchique.

---

### Outils utilisés
- **Tableau Public** — visualisation de données et création de tableaux de bord
- **Microsoft Excel** — classification des données et analyse par tableau croisé dynamique
