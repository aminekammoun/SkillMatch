Phase CRISP-DM	Description
1. Business understanding	
Question métier : Quelles compétences clés manquent sur le CV d'un candidat pour un poste ciblé ?


Indicateur de succès : Pertinence des recommandations jugée utile par l'utilisateur (taux d'acceptation > 75%).


Lien SMART : Atteindre un matching rapide et pertinent pour aider à l'insertion.

2. Data understanding	
Données nécessaires : CVs utilisateurs (PDF anonymisés), descriptions d'offres d'emploi (texte brut / JSON), référentiel de compétences (compétences techniques et soft skills).


Volume / Fraîcheur / Sensibilité : Données fictives ou échantillons locaux, faible volume, sensibilité personnelle (données de CVs).

3. Data preparation	
Problèmes attendus : Formats de CV hétérogènes (mises en page variées), fautes d'orthographe, bruits textuels, synonymes (ex: « MS PowerBI » vs « Power BI »).


Traitement : Normalisation du texte en minuscules, suppression des stop words, lemmatisation avec spaCy, extraction par expressions régulières et dictionnaire de compétences.

4. Modeling	
Modèle envisagé : Approche NLP déterministe et sémantique via TF-IDF et similarité cosinus via scikit-learn / spaCy.


Pourquoi pas d'IA générative ? Inutile pour ce MVP : un modèle de similarité textuelle est plus explicable, plus rapide à exécuter, moins coûteux et s'évalue beaucoup plus rigoureusement dans le cadre de CRISP-DM.

5. Evaluation	
Métrique technique : Score de similarité cosinus (seuil d'acceptation > 0.6 pour une correspondance pertinente).


Métrique métier : Pourcentage de compétences manquantes identifiées correctement par rapport à une analyse humaine de référence (objectif : > 80%).

6. Deployment	
Forme d'utilisation : Application web interactive (Frontend React, Backend FastAPI).


Maintenance : Assurée par l'équipe projet (mise à jour du référentiel de compétences et des offres de test).
