   SkillMatch - Charte de Projet

   1. Contexte et problème
-   La difficulté d'insertion professionnelle des jeunes diplômés réside souvent dans l'inadéquation ou la mauvaise valorisation de leurs compétences par rapport aux attentes réelles du marché. 
-   Question HMW :   « Comment pourrions-nous aider les étudiants et jeunes diplômés à identifier les compétences qui leur manquent par rapport aux attentes du marché de l'emploi afin de mieux préparer leur insertion professionnelle ? »
-   Insight :   Les candidats manquent d'outils analytiques objectifs pour auditer leur profil avant de postuler.

   2. Objectif SMART
-   Spécifique :   Développer un prototype fonctionnel de plateforme de matching CV/offres d'emploi capable d'extraire les compétences et d'afficher un plan de progression.
-   Mesurable :   Obtenir un score de précision d'extraction des compétences de l'ordre de 80% sur un jeu de test de 50 CVs et générer un matching en moins de 3 secondes.
-   Atteignable :   Grâce à une stack technique maîtrisée (Python, FastAPI, spaCy, React).
-   Réaliste :   Centré exclusivement sur l'analyse et le conseil (exclusion de la gestion des candidatures et de l'IA générative complexe).
-   Temporellement défini :   Livrable finalisé et déployé pour la fin de la séance académique.

   3. Périmètre (Scope)
-   Inclus :   Importation de CV PDF, extraction automatique des compétences, comparaison avec une offre d'emploi, calcul d'un score de correspondance, identification des lacunes et affichage de recommandations de formation.
-   Exclu :   Candidature automatique, mise en relation directe avec les recruteurs, gestion de candidatures, prédiction de l'obtention d'un emploi et génération automatique de nouveaux CVs.

   4. Parties prenantes (Matrice pouvoir / intérêt)
-   Étudiants / Jeunes diplômés (Pouvoir faible / Intérêt fort) :   Utilisateurs finaux. Stratégie : Impliquer via des tests utilisateurs et itérer sur l'ergonomie.
-   Équipe Projet / Étudiants MSc Data Management (Pouvoir fort / Intérêt fort) :   Conception et réalisation. Stratégie : Pilotage actif et partage des tâches via Git.
-   Enseignants / Jury (Pouvoir fort / Intérêt fort) :   Évaluation. Stratégie : Respect strict des exigences académiques et livrables normés.

   5. Approche et justification
-   Approche :   Méthode agile (type Scrum allégé) combinée à la méthodologie   CRISP-DM   pour la brique analytique. L'incertitude résidant dans la qualité de l'extraction des données non structurées (CVs), une démarche itérative par phases s'impose.

   6. Jalons clés
1. Cadrage et définition du besoin (Parties 1 à 3)
2. Modélisation et choix de l'architecture data (Partie 4 / CRISP-DM)
3. Spécification du MVP et User Stories (Partie 5)
4. Finalisation du dépôt GitHub et génération du Deck PDF (Partie 6)

     Arbitrage du Triangle d'Or
En cas de contrainte majeure, nous sacrifions le   délai   sur les fonctionnalités secondaires, en préservant en priorité la   qualité   de l'algorithme de matching et la   cohérence   de la proposition de valeur.
