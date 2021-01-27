# The_Product
Introduction
Le présent document présente une ébauche des spécifications fonctionnelles générales pour une plateforme de test en ligne. Il s’agit d’une application web qui permettra aux utilisateurs de passer des tests techniques en ligne, ou de proposer des tests à passer par d’autres utilisateurs.
Après la validation de ce document un autre document de spécifications fonctionnelles détaillés ainsi que des spécifications techniques devrait être fourni. Ce document après validation pourrait être enrichi avec des maquettes fonctionnelles (wireframes) ainsi que différents diagrammes (use case, activité, séquence, flux…)
Acteurs
Les acteurs de l’applications sont les suivants :
Anonyme : les utilisateurs anonymes peuvent accéder au site lire les pages « Accueil », « Qui sommes Nous », « Contact » etc. 
Pour accéder à l’espace candidat (et accéder aux tests) un acteur anonyme doit avoir un compte candidat ou créer un.
Pour accéder à l’espace entreprise un acteur anonyme doit avoir un compte entreprise ou créer un.
Membre Candidat : utilisateur inscrit en tant que candidat, il a le droit de passer des tests techniques. Il peut recevoir plusieurs tests par une ou plusieurs entreprises.
Entreprise : utilisateur ayant les droits de proposer des tests, et d’inviter par mail un candidat à passer un test existant. Une entreprise peut proposer autant de tests que son abonnement lui permet.
Modérateur : valider les tests proposés par les entreprises membres de la plateforme. 
Administrateur : gestionnaire de la plate-forme disposant d’accès avancés.


Front office
Dans cette partie nous allons présenter brièvement l’ensemble des fonctionnalités fournies par l’application aux différents acteurs du front office. 
Nous allons également voir avec plus de détails les fonctionnalités de gestion de compte ainsi que le processus de test et d’évaluation.
 Anonyme
Les principales fonctionnalités offertes pour cet acteur sont : 
Créer un compte (remplir un formulaire et valider son compte par mail
Se connecter (s’il dispose déjà d’un compte)
Passer un test (déclenche automatiquement la fonctionnalité se connecter / créer un compte),
Membre Candidat

Un membre candidat est un acteur qui s’est connecté avec un compte qu’il possède déjà (ou vient juste de le créer). Il peut ainsi :
Passer un test sur une technique de son choix
Passer un test auquel il a été invité par une entreprise
Entreprise
 Une entreprise est un acteur anonyme qui s’est connecté avec un compte entreprise qu’il possède déjà (ou vient juste de le créer). Il peut :
Créer et proposer des quizz ou des test
Inviter un candidat à passer un test déjà existant sur la plateforme
Création de compte candidat
La création de compte débutera par le remplissage d’un formulaire d’inscription.
Les informations suivantes seront demandées :
Nom et prénom
Email
Mot de passe avec confirmation
Activation du compte après la réception d’un mail de vérification
L’utilisateur est automatiquement connecté à son compte et redirigé vers la page à partir de laquelle il a souhaité s’inscrire.

Création de compte entreprise

La création de compte débutera par le remplissage d’un formulaire d’inscription.
Les informations suivantes seront demandées :
Nom de l’entreprise
Activité
Nombre d’employés
Nom de la personne qui crée le compte
Qualité de la personne qui crée le compte
Email
Mot de passe avec confirmation
Adresse mail
Documents à joindre à l’inscription (à préciser ultérieurement)
Activation du compte après la réception d’un mail de vérification
L’utilisateur est automatiquement connecté à son compte et redirigé vers la page à partir de laquelle il a souhaité s’inscrire.
Modification du compte
L’utilisateur peut à tout moment éditer les informations de son compte.

Processus de test

Avant de commencer le test le candidat est informé du sujet du test, du nombre de questions, du niveau du test et des trucs et astuces qui peuvent l’aider.
Une fois le test commencé le candidat réponds aux questions une à une en cochant les cases nécessaires. Si plusieurs réponses peuvent être correctes il en est informé.
A le fin du test le candidat est invité soit à réviser ses réponses soit à les valider définitivement et finir le test.
Dans le cas d’un candidat qui passe le test spontanément il obtient juste son score à la fin.
Pour les tests envoyés à travers une entreprise le candidat reçoit son score et l’entreprise reçoit un rapport détaillé sur son test, ses réponses et son activité pendant le test.
Back office
Dans cette partie nous allons présenter les fonctionnalités dédiées aux acteurs du back office qui sont l’administrateur et le modérateur. Nous allons également présenter la technique d’optimisation de recherche et de référencement SEO.
Administrateur
L’administrateur dispose d’accès avancés sur la plate-forme.
Ainsi il gère le contenu du site (contact, informations générales, ligne éditoriale …), il est également responsable du contenu du blog.
C’est l’administrateur qui crée le compte modérateur et dispose d’un tableau de bord qui lui permet d’avoir une vue globale du trafic du site (les fonctionnalités du tableau de bord seront détaillées dans la spécification technique détaillée)
Modérateur
Le modérateur, une fois connecté dispose des fonctionnalités suivants :
Valider un test
Désactiver un compte (pour mauvais usage)
Répondre aux réclamation
Valider un compte
Le modérateur dispose d’accès à un tableau de bord qui sera pareil à celui de l’administrateur ou avec des accès restreints, le choix sera fait lors de la rédaction des spécifications détaillées.
Il pourrait y avoir un seul compte Administrateur/modérateur (selon l’arbitrage qui sera fait avec le comité de pilotage)
SEO
La plateforme est optimisée pour les moteurs de recherche avec :
Gestion automatisée des « méta tags » (méta description, tag de partage Facebook, Twitter, etc.)
Gestion des alias automatiques
Gestion du fil d’ariane automatisé
Gestion des titres des balises pensé en amont
Gestion automatisée du plan du site
Mise en place de Google Analytics pour le suivi

3. Navigation

Arborescence
L’arborescence de l’application sera comme suit :
Accueil
Qui sommes nous?
Freelance
Nous rejoindre
Trouve une mission
Apporter une affaire
Développeur
Teste tes compétences
Trouve un emploi
Entreprise
Recrutez
Evaluez vos candidats
Trouver un freelance
Login
Page d’accueil
La page d’accueil comporte tous les éléments nécessaire pour les visiteurs afin de comprendre le fonctionnement du produit.
Un slogan d’accroche avec un bouton pour créer un compte
Une présentation des services proposés 
Quizz
Résolution d’exercices de codage
Compétitions / challenges
Un champ pour s’abonner à la newsletter
Nos contact (mail / réseaux sociaux / adresse / téléphone)

Tri
Il est possible de trier les tests sur les critères suivants :
Catégorie
Type
Difficulté
Date d’ajout

Pages institutionnelles 
Les pages institutionnelles disposent d’une mise en page fixe. Elles peuvent être librement créées et attachées à un menu (principal ou pied de page).
Elles vont regrouper les mentions légales, conditions générales, etc. Elles peuvent aussi contenir quelques informations que ce soit en fonction des besoins.
Il est possible d’y insérer des images ou des vidéos Youtube.
