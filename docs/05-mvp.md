1. Hypothèse la plus risquée
« Nous pensons que les étudiants en fin d'études vont utiliser un outil d'analyse de CV pour identifier leurs lacunes techniques parce qu'ils doutent de leur adéquation avec les offres du marché. Nous le saurons si au moins 70% des utilisateurs testeurs suivent au moins une recommandation de formation affichée à la suite du matching. »

2. Forme du MVP
Un prototype cliquable (ou service web simple) permettant d'importer un PDF, de lancer l'analyse textuelle et d'afficher instantanément un score de correspondance avec une liste claire de 3 compétences manquantes et des liens vers des ressources.

3. Story Map (Parcours utilisateur)
Étape 1 : Importation

Story 1.1 : Importer son CV au format PDF.

Étape 2 : Analyse

Story 2.1 : Extraire automatiquement les compétences techniques du CV.

Story 2.2 : Sélectionner une offre d'emploi cible.

Étape 3 : Résultat & Progression

Story 3.1 : Afficher un score de correspondance global.

Story 3.2 : Lister les compétences maîtrisées et manquantes.

Story 3.3 : (Responsabilité) Afficher une case de consentement explicite et garantir la non-conservation des données personnelles. (Ligne de découpe du MVP traversant toutes ces étapes).

4. User Stories au format Given / When / Then
User Story 1 : Importation et extraction

En tant qu' étudiant en recherche d'emploi, je veux importer mon CV au format PDF afin d' extraire automatiquement mes compétences techniques.

Critères d'acceptation :

Étant donné que je suis sur la page d'accueil, lorsque je glisse-dépose un fichier PDF valide, alors le système extrait le texte et affiche un message de succès.

Étant donné un fichier non PDF, lorsque je tente l'importation, alors un message d'erreur explicite s'affiche.

(Donnée liée : PyMuPDF / Phase 2 Data Understanding).

User Story 2 : Matching et identification des écarts

En tant qu' utilisateur, je veux comparer mon profil à une offre d'emploi sélectionnée afin d' obtenir mon score de correspondance et mes lacunes.

Critères d'acceptation :

Étant donné que mon CV est analysé, lorsque je sélectionne une offre d'emploi et clique sur "Lancer le matching", alors la plateforme affiche un score en pourcentage et classe les compétences en "Maîtrisées" et "Manquantes".

Étant donné un profil sans compétences détectées, lorsque je lance le matching, alors une alerte m'invite à vérifier la structure de mon CV.

(Donnée liée : Algorithme TF-IDF / Phase 4 Modeling).

User Story 3 : Responsabilité et RGPD (Story obligatoire)

En tant qu' utilisateur soucieux de la confidentialité, je veux être informé de l'utilisation de mes données et donner mon consentement afin de protéger ma vie privée.

Critères d'acceptation :

Étant donné l'importation d'un CV, lorsque j'arrive sur l'interface d'upload, alors une mention explicite m'informe que les données ne sont pas stockées à des fins commerciales.

Étant donné la fin de la session, lorsque je ferme la page, alors mon CV est immédiatement supprimé du serveur.

(Donnée liée : Respect RGPD / Phase 2 Sensibilité des données). 
