🎓 **Projet Ontologie – Domaine de l'Éducation**

📘 **Description du projet**

L'éducation, en tant que secteur en constante évolution, génère une multitude d'informations concernant les étudiants, enseignants, départements et cours, informations essentielles au bon fonctionnement des institutions académiques. Avec l'augmentation des systèmes numériques et des plateformes éducatives, la gestion des données devient un véritable défi, car elles proviennent de sources diverses, telles que les inscriptions, les évaluations, les emplois du temps, etc. Cependant, ces données sont souvent dispersées, non structurées et difficiles à exploiter efficacement.
L'objectif est de faciliter l'accès et la gestion des informations pour les différents acteurs du système éducatif (étudiants, enseignants, gestionnaires). 
Ce projet consiste à créer une ontologie pour le domaine de l'éducation, en utilisant des technologies sémantiques comme RDF, RDFS, OWL et SPARQL. L'ontologie structure les données relatives aux individus (étudiants, enseignants), aux structures académiques (départements, modules de cours), aux événements académiques (évaluations, semestres), et à l'organisation spatiale (salles). 

Le projet a été développé avec l'outil **Protégé**, en utilisant des namespaces standards pour garantir l'interopérabilité et la réutilisation des données.

🎯 **Objectifs du projet**
- Modéliser les entités du domaine de l'éducation sous forme d'ontologie.
- Permettre l’inférence de nouvelles connaissances à partir des faits existants.
- Utiliser RDF, RDFS, OWL et SPARQL pour la gestion et la requête des données.
- Appliquer des namespaces standards tels que XML Schema, Dublin Core, FOAF, SKOS, RDFS, et OWL pour structurer et enrichir les données.
- Faciliter l'accès aux informations académiques et améliorer l'interopérabilité des systèmes éducatifs.

🧠 **Apports de l'ontologie**
1. **Inférence de connaissances** : Grâce aux règles SWRL et aux capacités d'inférence d'OWL, l'ontologie peut déduire de nouvelles relations qui ne sont pas explicitement définies. 
2. **Flexibilité du modèle** : L'ontologie permet d'ajouter de nouveaux concepts et relations sans avoir à restructurer l'ensemble du modèle.
3. **Interopérabilité** :  L’utilisation des standards du Web Sémantique permet une intégration facile avec d’autres sources de données.
4. **Richesse sémantique** : L'ontologie capture non seulement les données, mais aussi leur signification et leurs relations.
5. **Requêtes complexes** : SPARQL permet d’interroger des relations directes, indirectes et inférées, difficilement faisables avec SQL.
Cette ontologie offre une vue globale et structurée des entités éducatives et leurs interactions.

🛠️ **Technologies utilisées**
- **Protégé** est un Outil de développement pour les ontologies.
- **RDF** (Resource Description Framework) est un modèle de données pour la description des ressources et des relations entre elles.
- **RDFS** (RDF Schema) est un vocabulaire pour définir les relations entre les ressources RDF.
- **OWL (Web Ontology Language)** est un langage de modélisation sémantique qui permet de définir des ontologies et des relations complexes entre les concepts.
- **SPARQL** est un Langage de requête pour interroger les données RDF.
- **SWRL (Semantic Web Rule Language)** est un langage qui permet d’exprimer des règles logiques sous forme d’implications afin d’inférer de nouvelles connaissances à partir des faits déjà présents dans l’ontologie.

🧭 **Namespaces utilisés**
- **xsd (XML Schema)** définit les types de données XML : [http://www.w3.org/2001/XMLSchema#]
- **dc (Dublin Core)**  est un ensemble de métadonnées standardisé pour décrire les ressources sur le web, y compris le titre, l'auteur, la date, etc : [http://purl.org/dc/elements/1.1/]
- **FOAF (Friend of a Friend)** est un vocabulaire RDF utilisé pour décrire des personnes, leurs relations et leurs activités sur le web : [http://xmlns.com/foaf/0.1/]
- **SKOS (Simple Knowledge Organization System)** est un modèle RDF pour représenter des vocabulaires contrôlés et des thésaurus, facilitant l'organisation des connaissances. : [http://www.w3.org/2004/02/skos/core#]
- **RDFS** est un vocabulaire RDF utilisé pour définir des classes, des propriétés et des relations entre les ressources : [http://www.w3.org/2000/01/rdf-schema#]

💻 **Installation et utilisation**
✅ Prérequis
Avant de pouvoir utiliser le projet, vous devez installer **Protégé**, un outil qui vous permet de visualiser et de manipuler des ontologies.
🔽 Installation de Protégé
🔗 Télécharger depuis : protege.stanford.edu
🖥️ Installer selon votre système (Windows/macOS/Linux)

📂 Importation de l'ontologie dans Protégé
1. Ouvrir Protégé.
2. Aller dans File > Open.
3. Télécharger le fichier .rdf depuis le dépôt GitHub.
4. Charger le fichier.
🎉 Visualisez la structure (classes, propriétés, graphes, inférences…).

🔍**Visualisation**
Dans Protégé, vous pouvez :
- Voir les classes (`Étudiant`, `Enseignant`, etc.).
- Explorer les instances (individus concrets).
- Examiner les propriétés reliant les entités.
- Visualiser des graphes relationnels.
- Écrire et exécuter des requêtes SPARQL pour interroger les données.
📄 Note : Un fichier nommé requêtes_sparql.txt contenant plusieurs exemples de requêtes SPARQL est déjà présent dans ce dépôt.
Tu peux le consulter pour explorer l’ontologie directement depuis Protégé.

⚙️**Règles SWRL et Raisonnement avec Pellet**

Vous pouvez également définir des règles SWRL (Semantic Web Rule Language) pour enrichir votre ontologie avec des règles logiques. Ces règles permettent de déduire de nouvelles connaissances à partir des faits existants.
Pour visualiser les résultats des règles SWRL et les types inférés, vous devez utiliser un raisonneur compatible, notamment Pellet.

📌 Remarque : Les règles SWRL ne fonctionnent qu’avec le raisonneur Pellet.

✅ Installation du plugin Pellet dans Protégé :
   1. Ouvrez Protégé.
   2. Allez dans File > Check for plugins.
   3. Recherchez Pellet Reasoner dans la liste.
   4. Cochez-le et cliquez sur Install.
   5. Redémarrez Protégé.
   6. Activez-le ensuite via le menu Reasoner > Pellet Reasoner, puis cliquez sur Start reasoner.

📦 **Clonage du projet**
Pour cloner ce projet, suivez ces étapes :
1. Ouvrez votre terminal ou invite de commande.
2. Exécutez la commande suivante pour cloner le dépôt :
   ```bash
   git clone https://github.com/OumaymaKhlif/University-Ontology-Project.git
   
✨ **Auteurs**

Oumayma Khlif

Saba Kallel
