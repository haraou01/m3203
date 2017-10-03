# TP 3 : Interfaces

## Cours

**Interface** : Une interface ne possède ni propriétés, ni définition de méthodes. Elle ne contient que la déclaration de méthodes. Il est ainsi possible de "passer un contrat de développement" dans lequel une classe qui implémente une interface aura pour obligation qu’elle définisse les méthodes. Donc, en tant que développeur, on s’engage à définir convenablement les méthodes déclarées dans l’interface. Si, on venait à ne pas respecter cet engagement, PHP nous le signalerait par une erreur.

**Interface multiple** : une classe peut implémenter plusieurs interfaces.

**Méthodes** : une classe qui implémente une interface peut déclarer et définir des méthodes qui ne figurent pas dans l’interface.

**Convention de nommage** : le nom de l’interface a pour initiale la lettre i minuscule.

### Exemple de code

Soit la classe Personne et une interface iPersonne



Soit une application instanciant la classe Personne



L’exécution de cette application provoquera l’erreur suivante


car les méthodes sePresente() et travaille() n’ont pas été définies dans la classe Personne. Le contrat n’a pas été respecté !

Nous pourrions proposer ce code :


##	Exercice

Nous vous proposons d’analyser le code ci-dessous puis de l’écrire pour le tester.
Puis ajouter la déclaration public function ajoutsaut() ; dans l’interface et tester à nouveau.

Code de html.php

Code de td7.php

