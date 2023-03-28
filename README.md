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

### Quelle est la différence entre `let` et `var` ?

- `let` permet de créer une valeur constante après initialisation.
- `var` permet de créer une valeur qui peut changer à tout moment.

La différence entre `let` et `var` est ici la mutabilité d'une valeur tout au long de l'exécution du programme. 

### Qu'est-ce qu'un optionnel ?

Un optionnel est une constante ou variable qui peut contenir ou non une valeur. Ils sont utilisés pour représenter des valeurs qui peuvent être absentes à un moment donné (`nil`).

Un optionnel se déclare avec `?`, et doit être assigné à une valeur ou `nil` si c'est une constante. Lorsqu'on souhaite accéder à son contenu, on peut y accéder avec:
- L'unwrapping (déballage)
- l'optional chaining
- L'optional binding
- Le nil coalescing avec `??`

### Qu'est-ce que l'optional chaining (chaînage d'optionnels) ?

L'optional chaining permet de manipuler des propriétés et des méthodes d'un objet optionnel de manière sûre et concise.

L'optional chaining permet d'accéder à une propriété ou d'appeler une méthode sur un objet optionnel sans avoir besoin de le déballer (unwrapping) en utilisant un opérateur de chaînage.

Si l'objet optionnel a une valeur, l'appel de la propriété ou de la méthode est effectué normalement. Si l'objet optionnel n'a pas de valeur, l'appel est simplement ignoré et retourne `nil`.

L'optional chaining s'effectue avec l'opérateur de chaînage `?` ou de manière forcée `!` (au risque d'un crash si c'est `nil`).

### Qu'est-ce que l'optional binding (liaison d'optionnel) ?

L'optional binding est une fonctionnalité du langage Swift qui permet de déballer (unwrapping) en toute sécurité des objets optionnels et de les assigner à des variables ou des constantes.

L'optional binding est souvent utilisé en conjonction avec la déclaration if let ou guard let. Ces déclarations permettent de vérifier si un objet optionnel a une valeur ou pas. Si l'objet a une valeur, il est déballé et assigné à une variable ou une constante. Si l'objet n'a pas de valeur, la déclaration est simplement ignorée.

### Qu'est-ce que le nil coalescing ?

Le `nil` coalescing est un opérateur qui garantit que l'optionnel contient une valeur. Avec `??`, l'optionnel déballe (unwrappe) sa valeur si elle est présente ou retourne une valeur par défaut si l'optionnel est `nil`.

### Qu'est-ce que la propriété `lazy` ?

Une propriété `lazy` est un atrribut d'une classe ou d'une structure en Swift qui n'est pas initialisé tant qu'il n'est pas utilisé pour la première fois. 

Les propriétés `lazy` sont utiles pour les propriétés qui sont coûteuses à initialiser ou qui ne sont pas nécessaires dans tous les cas d'utilisation. Elles permettent donc d'optimiser les performances du code.

Une propriété de ce type-là se déclare avec le mot-clé `lazy` et doit être une variable car sa valeur peut être modifiée dès son initialisation.

## <a name="git"></a>Questions sur Git

### Quelles sont les 3 commandes de fusion ?

Les 3 commandes de fusion sont les suivantes:
- `git cherry-pick`
- `git merge`
- `git rebase`

### Que fait la commande `git rebase` ?

`git rebase` est une commande avancée de fusion qui permet de réécrire l’historique d'une branche en appliquant les commits de l’autre branche, après ceux de la branche actuelle. Cela permet de garder un historique de développement propre et lisible.

### Quelle est la différence entre `merge` et `rebase` ?

La différence entre `git merge` et `git rebase` réside dans la façon où les modifications de 2 branches sont fusionnées.

`git merge` va créer un nouveau commit de fusion qui combine les modifications de deux branches. Cela peut entraîner une historique de développement avec des branches qui se croisent et des commits de fusion qui peuvent rendre l'historique plus difficile à suivre.

En revanche, `git rebase` réécrit l'historique de la branche en replaçant les commits de la branche courante sur le dessus de la branche cible. Cela crée une historique de développement linéaire et plus facile à suivre. En effet, cela permet de garder l'historique des commits propre et facilement compréhensible.

### Que fait la commande `git cherry-pick` ?

`git cherry-pick` permet d'appliquer les modifications d'un commit spécifique d'une branche à une autre branche en y créant un nouveau commit.

### Qu'est-ce que Gitflow ?

Gitflow est un modèle de branching Git alternatif qui utilise des branches de fonctionnalité et plusieurs branches primaires. Il permet un flux de travail efficace et collaboratif pour les projets de développement logiciel.

Gitflow se met en application avec 2 branches principales qui sont `main`/`master` (production) et `develop` (développement). On utilise des branches de fonctionnalité qui sont:
- `feature`: Une feature non finie qui sera mergée dans `develop`
- `release`: La prochaine release à partir en production (elle sera mergée dans `master`/`main` une fois en production)
- `hotfix` : Lorsqu'il y a un bug urgent à corriger (c'est comme une release sauf qu'elle part de `master`/`main` et non de `develop`)
