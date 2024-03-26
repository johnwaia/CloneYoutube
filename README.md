# **PROJET DEVELOPPEMENT WEB & MICRO-SERVICE 2024 :**
## **Clone de youtube**

## Table des matières
* [Implémentation Fonctions](#Fonctions-minimales-à-implémenter)
* [Critère d'évaluations](#Quelques-critères-d'évaluation)
* [Technologie](#Quelques-technologies-pour-le-développement)
* [Eclaircissement](#Quelques-technologies-pour-le-développement)
    * [OAuth2](#C'est-quoi-**OAuth2**)
    * [OpenId Connect](#C'est-quoi-**OpenId-Connect**)
    * [Docker Compose](#C'est-quoi-**Docker-Compose**)
        * [Docker](#Pour-commencer-:-**Docker**)
        * [Docker Compose : C'est quoi?](#**Docker-Compose**)

### Fonctions minimales à implémenter
Voici une liste des fonctions minimales à implémenter :
* **Upload d'une vidéo**, avec titre et une description
* Ajout d'une **section commentaire**
* **Système d'authentification** basé sur **OAuth2** & **Openld Connect**
* Lancement de l'application via Docker-Compose

### Quelques critères d'évaluation
La note se basera sur les critères d'évaluation ci-dessous :
* Implémentation des **fonctions minimales**
* Soin apporté à **l'implémentation** (Factorisation du code, Optimisation, Lisibilité etc.)
* Soin apporté à **l'interface graphique**
* **Documentation** associé au projet

### Quelques technologies pour le développement
Voici une liste non-exhaustive des technologie qu'il sera possible d'utiliser pour le développement de l'application web.
Ceci ne sont que des exemples de ce qu'il sera possible d'utiliser. Il n'est pas obligatoire de choisir les technologies parmi celles
cités ci-dessous.

### Eclaircissement
Cette partie est réservé à l'explication des différentes thématiques et technologie utilisé et abordé pour le développement du projet web.
Elle permettra aux développeurs et lecteurs du repos de mieux comprendre les rouages et mécanisme de l'application
* #### C'est quoi **OAuth2**
OAuth2 est un protocole permettant de déleguer un certain nombre d'autorisation à une application cliente, pour pouvoir accéder au ressources d'une entité (utilisateur etc.). Dans un schéma classique, les protocoles d'authorisation et d'authentifications font intervenir 2 parties :
* **Un serveur** en mesure d'identifier et d'authentifier l'accès à une ressource.
* **Un utilisateur** qui fournit des identifiants pour accéder à la ressource.
En ce qui concerne le protocole d'authorisation OAuth2 nous avons 4 acteurs qui entre dans le processus d'authenetification :

* #### C'est quoi **OpenId Connect**
* #### C'est quoi **Docker Compose**
    * #### Pour commencer : **Docker** 
    [Docker](https://www.docker.com/) est une plateforme permettant la conteneurisation de plusieurs applications et micro-service. Pour rappel un conteneur est un environnement d'éxécution contenant tout ce dont une application à besoin afin de fonctionner : dépendance, bibliothèque, code, variables d'environnement etc. Docker
    est l'une des solutions de conteneurisation les plus populaire sur le marché. Nous verrons plus tard comment télécharger Docker et comment nous nous en sommes servis pour déployer notre application web (*clone de youtube*).
    * #### **Docker Compose**
    Nous avons précédemment vu que Docker est utilisé pour déployer des applications fonctionnant indépendement l'une de l'autre. Mais comment procède-t-on pour le déploiement d'applications utilisant plusieurs micro-service. C'est la qu'intervient [Docker Compose](https://docs.docker.com/compose/). Il nous permettra d'orchestrer, de structurer les interactions entre les différents micro-service (applications). Par exemple nous souhaitons déployer un site wordpress avec une base de données. Nous déploierons donc un conteneurs pour le site wordpress et un autre conteneurs pour le le micro-service gérant la base de données qui va communiquer avec notre premier conteneurs. Nous verrons plus tard en détail le fonctionnement des interactions entre les conteneurs ainsi que leur déploiement, l'installation, et le configuration du Docker Compose.

