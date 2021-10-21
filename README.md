Projets : Modéliser un système de BI
  
Modéliser un système de BI
1. Introduction
Pour concevoir une bonne base de données, il faut bien comprendre le business concerné. Donc on fera souvent appel au Data Analyst pour réaliser la modélisation de la base ou pour vérifier que rien n'a été oublié. Avant que ça soit ton tour, profite de ce projet pour t'exercer et devenir un as de la modélisation de systèmes d'info décisionnels 🦁

2. Le projet
2.1. Un système d'info décisionnel pour votre université 🎓🎓
Maintenant que vous savez cruncher les classements mondiaux des universités, vous avez pu transmettre un reporting sur l'évolution des performances de votre Université. Depuis, les équipes veulent améliorer cette performance. Et pour cela, le recteur de l'Université de Strasbourg vous a demandé de mettre en place un système qui lui permettra de prendre des décisions éclairées.

En fait, il cherche à étudier les facteurs influant sur la réussite des candidats aux examens. Pour cela, on vous a chargé de construire un datawarehouse.

Il souhaite pouvoir répondre aux questions suivantes :

Quel est le nombre de réussites aux examens par cours, pour l’année 2020 ?
Quel est le nombre de réussites aux examens d’un cours obligatoire, pour l’année 2020 ?
Quel est le nombre de réussites aux examens par genre (féminin, masculin), entre 2019 et 2020 ?
Combien d’apprenants ayant un âge supérieur à 23 ans ont réussi leurs examens de « BI » ?
Quel est le nombre de réussites aux examens pendant le semestre d’hiver 2020 ?
Pour cela, vous disposez des données suivantes :
Pour chaque examen passé, on connaît l’âge et le genre de l’apprenant, le nom du cours (les cours peuvent être regroupés en cours obligatoire et cours à option), la date de l’examen, la note obtenue et si l’examen est réussi ou non.

Pour l'instant, il vous demande de réfléchir à la conception du système. Vos premières missions sont les suivantes :

Donner la table principale de l’entrepôt ainsi que les tables dimensions relatives.
Tracer le schéma en étoile dimensionnel.
2.2. Un système décisionnel pour étudier vos ventes 💰💰
Un ami à vous possède une entreprise qui revend du matériel informatique. Il vous demande de l'aider dans la gestion de ses ventes car il n'arrive pas vraiment à piloter son entreprise pour l'instant.

La seule chose dont il dispose est d'un fichier Access qui contient sa base de données.

Pour aider votre ami, vous allez utiliser le logiciel PowerBI Desktop (à télécharger ici).
Vous importez votre fichier sales.db, vous chargez toutes les tables.

Pour en savoir plus sur le fonctionnement de PowerBI, vous pouvez regarder cette vidéo ou la doc de Microsoft.

Vos missions sont les suivantes :

Déterminer la table fait et les tables dimensions
Créer un modèle relationnel en Etoile
Créer un modèle relationnel en Flocon
Ajouter deux nouvelles mesures : Total_Sales, Total_Costs
Afficher les totaux des ventes par client et par date
Visualiser la moyenne des ventes par catégorie de produit
3. Rendu attendu
Un fichier .pdf contenant les schémas de l'exercice 1.
Un fichier .pbix contenant le schéma et les ajouts effectués sur vos tables de données pour l'exercice 2.

___________________________________


Projets : Jouer avec une base NoSQL
  
Jouer avec une base NoSQL
Ca c'est vraiment la classe 🔮🔮

1. Introduction
Dans ce projet, tu vas utiliser MongoDB 🎉🎉 Développé en 2007, MongoDB est depuis devenu un des SGBD les plus utilisés. Selon le classement DB-Engines Ranking, MongoDB se classe en cinquième position des serveurs de données les plus populaires au niveau mondial. Première technologie NoSQL de ce palmarès, l'infrastructure open source de MongoDB se hisse juste derrière les principaux systèmes phares de base relationnelle : Oracle Database, MySQL, SQL Server et PostgreSQL - avec lequel elle est au coude-à-coude.

ranking

2. Le projet
2.1. Créer un cluster sur MongoDB Atlas
Un cluster est un groupe de deux ou plusieurs serveurs indépendants fonctionnant comme un système unique.
Et MongoDB Atlas est une version cloud entièrement gérée de la base de données. Cela va nous aider car autrement, les tâches nécessaires, telles que l’installation de la base de données, son réglage pour maintenir des performances optimales sur de longues périodes et sa sécurisation, ont tendance à demander beaucoup d’efforts spécialisés ...

Avec MongoDB Atlas, tu vas pouvoir créer un cluster MongoDB auprès de tout fournisseur de cloud majeur de votre choix et commencer à utiliser ce cluster en quelques minutes.

Tout d'abord, tu dois te créer un compte sur MongoDB Atlas.
Ensuite, tu te connectes, tu crée un cluster et tu lui donnes un nom. Choisis la version Free.
Puis, tu crées un utilisateur de base de données.
Tu ajoutes les adresses IP qui peuvent se connecter à ta base de données. Choisis que le serveur est accessible partout.
Tu connectes le cluster à MongoDB Compass.
2.2. Télécharger MongoDB Compass
Télécharge l'outil graphique MongoDB Compass, tu l'ouvres et tu le connectes à ton cluster en collant l'url de connexion obtenu précédemment (en changeant 'password' par le mot-clé qui avait été saisi lors de la création de l'utilisateur.
Crée une base de données 'demo' et une collection 'publis'.
Télécharge les données disponibles ici. Il s'agit d'un extrait de la base de données DBLP (Digital Bibliography & Library Project), un catalogue de bibliographies en informatique disponible en ligne.
Dézippe le fichier et importe le à ta base de données.
2.3. Requêter la base de données
Ca y est tu as maintenant une base de données disponible sur MongoDB. A toi de faire les requêtes suivantes :

Vérifier le nombre de documents importés.
Prévisualiser les 20 premiers documents.
Lister tous les livres (type 'Book').
Lister les publications depuis 2011.
Lister toutes les publications de 2011 et 2013.
Lister toutes les publications de 2011 ou 2013.
Lister les publications ayant 3 auteurs.
Lister les livres publiés depuis 2014.
Lister les publications de l'auteur "Toru Ishida".
Lister tous les éditeurs (type 'publisher') distincts.
Lister tous les auteurs distincts.
Trier les publications de 'Toru Ishida' par titre de livre et par page de début.
Compter le nombre de ses publications.
Compter le nombre de publications depuis 2011 et par type.
Compter le nombre de publications par auteur et trier le résultat par ordre croissant.
Aide ici.

3. Rendu attendu
Un fichier texte qui donne l'ensemble des requêtes pour obtenir les réponses.