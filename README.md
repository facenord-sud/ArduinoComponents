# ArduinoComponents
> Ensemble de classes Java représentant des composants Arduino

## Description
Cette bibliothèque est destinée à être utiilisée en interaction avec [ArduinoCommunication](https://github.com/facenord-sud/ArduinoCommunication)
L’idée est simple. Nous partons du principe qu'une classe Java représente un composant Arduino et qu’il existe un nombre limité de composants Arduino. L’idée est de rassembler toutes les classes de composants Arduino. Ainsi, au fur et à mesure que le nombre de projets, suivant la même structure que le nôtre, augmentera, il sera possible d’utiliser n’importe quelle classe Java représentant un composant sans avoir à le recréer à chaque fois.

À chaque fois qu’un composant Arduino n’a pas d’équivalent Java, l’idée est de le créer et de l’ajouter à la bibliothèque. Ainsi, au fur et à mesure des projets, cette bibliothèque s’aggrandira. Cependant, c’est une idée expérimental et des propositions de modifications et d’améliorations sont les bienvenues.

## Motivation
La motivation est de pouvoir gagner du temps durant le processus de développement de l’application en utilisant du code existant. Pour chaque application du Web des Objets, il est possible d’imaginer que les composants Arduino utilisés sont pratiquement les mêmes. De plus, créer à chaque fois les mêmes classes représentant les composants est un travail ennuyeux et inutil. Imaginez une dizaine de projets utilisant tous un composant de type moteur à rotation continue. Sans cette librairie, cela signifie qu’une dizaine de classes quasiment identiques sont créées, représentant toutes un moteur à rotation continue. De plus, si nous partons du principe qu’un développeur crée plusieurs applications et qu’un développeur est de nature flemmarde, il aura tôt fait d’effectuer du copier-coller pour éviter de devoir écrire du code. Si, le même développeur remarque qu’il manque une fonctionnalité ou un bug dans une des classes de composant. Il devra modifier manuelle- ment toutes les classes. Scénario plutôt horrible, non ? Surtout si au lieu d’une dizaine de projets, on parle d’une centaine...

C’est pourquoi, notre solution permettrait de résoudre le problème posé ci-dessus. Comme tout le monde, dans tous le projets, utilise les même classes, un bug ou une fonctionnalité manquante dans une des classes peut être corrigé rapidement et être effectif dans tous les projets.

Coupler un logiciel de contrôle de version de type Git et de rendre cette bibliothèque publique sur un site tel que Github, améliorerait encore sa facilité d’utilisation. Permettant ￼à chacun d’ajouter et de modifier une classe de composants. C’est la dernière motivation pour cette bibliothèque, un même code utilisé, testé et relu par un grand nombre de personnes ne peut être que meilleur que le code développé par un seul programmeur.


## Utilisation

Comme il est prévu de distribuer cette bibliothèque sous forme de dépendance Maven, il suffit de l’inclure dans le fichier pom.xml puis d’utiliser les classes qu’elle contient pour interagir avec l’Arduino.

Pour ajouter ou modifier une classe de composant le processus est simple et commun à beaucoup de projets open-source sur Github :

1. Forker le projet
2. Modifier selon ses désirs le répertoire
3. Soumettre une requête pull

Puis les personnes responsables du répertoire Github, contrôlent les modifications, en discutent avec la personne ayant proposé des modifications et avec la communauté. Si la modification fait sens, la requête pull est accepté et les nouveaux changements disponibles pour tous les utilisateurs de la dépendance. La seul nécessité étant d’avoir une équipe pour gérer le projet suffisamment grande, disciplinée et réactive pour répondre efficacement aux requêtes pull.
