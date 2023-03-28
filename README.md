# Cheat sheet questions entretien développeur iOS

Voici un cheat sheet comportant des questions à laquelle un développeur iOS doit être capable de répondre de manière simple, claire et efficace lors d'un entretien technique pour un recrutement ou un staffing chez un client.

Ce format d'entretien est une épreuve de communication et de savoir-faire technique, en situation de stress, le tout en très peu de temps.

## Table des matières
- [Questions générales de programmation](#general)
- [Questions sur les design patterns](#designpatterns)
- [Questions sur le langage Swift](#swift)
- [Questions Git](#git)

## <a name="general"></a>Questions générales de programmation

### Qu'est-ce que la programmation orientée objet ?

La programmation orientée objet (POO) est un paradigme de programmation dans lequel les données et le code qui les manipule sont regroupés en objets.

Un objet est une instance d'une classe qui encapsule des données et des méthodes. Les données sont représentées par des attributs et les méthodes sont des fonctions qui permettent de manipuler ces données. L'objectif de la POO est de modéliser le monde réel de manière plus intuitive et de faciliter la réutilisation et la maintenance du code.

### Qu'est-ce qu'une classe ?

Une classe est un modèle qui définit les attributs (variables) et les méthodes (fonctions) qui caractérisent un ensemble d'objets. Autrement dit, une classe est un modèle pour créer des objets de même type. Les attributs représentent l'état ou les caractéristiques de l'objet, tandis que les méthodes représentent le comportement ou les actions que l'objet peut effectuer.

### Quelles sont les principales caractéristiques de la programmation orientée objet ?

Les principales caractéristiques de la programmation orientée objet sont les suivantes:
- Encapsulation
- Abstraction
- Polymorphisme
- Héritage

### Qu'est-ce que l'encapsulation

L'encapsulation est un mécanisme consistant à rassembler les attributs et les méthodes au sein d'une structure en cachant les détails de son implémentation.

L'encapsulation permet de protéger les données et les méthodes d'un objet contre les accès non autorisés ou les manipulations imprévues, ce qui améliore la sécurité et la fiabilité du code. Elle facilite également la maintenance du code.

### Qu'est-ce que l'héritage ?

L'héritage est un mécanisme qui permet à une classe d'hériter des attributs et méthodes d'une autre classe appelée classe parent ou super classe.

En héritant de la classe parent, la sous-classe ou classe dérivée peut réutiliser le code de la classe parent sans avoir besoin de le réécrire. Elle peut également ajouter ses propres attributs et méthodes spécifiques, et modifier ou surcharger les méthodes de la classe parent pour les adapter à ses propres besoins.

### Qu'est-ce que le polymorphisme ?

Le polymorphisme est un concept de la programmation orientée objet (POO) qui permet à un objet de prendre plusieurs formes ou comportements. Plus précisément, le polymorphisme permet à des objets de différentes classes d'être traités de la même manière en utilisant des méthodes qui ont la même signature, c'est-à-dire le même nom et les mêmes paramètres, mais qui peuvent avoir des implémentations différentes pour chaque classe.

### Qu'est-ce que l'abstraction ?

En programmation orientée objet, l'abstraction est le processus de capture des caractéristiques essentielles d'un objet sans tenir compte des détails non essentiels. Cela permet de modéliser un objet ou un système de manière plus simple et plus compréhensible, en se concentrant sur les aspects pertinents pour la tâche à accomplir, et en masquant les détails complexes qui ne sont pas nécessaires.

L'abstraction est souvent réalisée en créant des classes et des interfaces qui définissent les propriétés et les comportements d'un objet, tout en cachant les détails d'implémentation sous-jacents. Par exemple, une classe "Voiture" peut être utilisée pour représenter les voitures dans un programme, en fournissant des méthodes telles que "démarrer", "accélérer", "freiner", etc., tout en masquant les détails de l'implémentation tels que le fonctionnement du moteur, la transmission, etc.

L'abstraction est un concept clé de la POO car elle permet de modéliser des systèmes complexes en les simplifiant, en réduisant la complexité de la conception, en améliorant la lisibilité et la maintenabilité du code. Elle permet également de créer des classes et des interfaces génériques et réutilisables, qui peuvent être utilisées dans différents contextes sans avoir besoin de connaître les détails de leur implémentation interne.

## <a name="designpatterns"></a>Questions sur les designs patterns

### Qu'est-ce qu'un design pattern ?

Un design pattern est une solution éprouvée et réutilisable à un problème commun de conception de logiciel. Il s'agit d'un modèle général de conception de code qui peut être adapté et réutilisé dans différents projets pour résoudre des problèmes similaires.

Les design patterns sont souvent utilisés pour résoudre des problèmes de conception courants dans la programmation orientée objet, tels que la création d'objets, la gestion des relations entre les objets, la structuration du code, la gestion des erreurs, etc.

Ils permettent de produire un code plus clair, plus maintenable et plus réutilisable, tout en réduisant les erreurs et en améliorant l'efficacité du développement de logiciels.

### Qu'est-ce que l'injection de dépendances ?

L'injection de dépendances est un pattern où un objet reçoit d'autres objets dont il dépend.

La classe dépendant ici d'une abstraction, l'injection d'une dépendance peut s'effectuer de l'extérieur de 3 façons:
- Initialiseur
- Méthode
- Propriété (affectation directe)

L'injection de dépendances permet de réduire le couplage, d'avoir un code réutilisable, testable et maintenable.

## <a name="swift"></a>Questions sur le langage Swift

## <a name="git"></a>Questions sur Git

### Que fait la commande `git rebase` ?

### Quelle est la différence entre `merge` et `rebase` ?
### Que fait la commande `git cherry-pick` ?

`git cherry-pick` permet d'appliquer les modifications d'un commit spécifique d'une branche à une autre branche en y créant un nouveau commit.