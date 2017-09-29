# TD N°4 : Héritage multiple

## Cours

### Héritage multiple

L’héritage est le moyen de spécialiser une classe sans compromettre son code original. PHP autorise l’héritage 
multiple. Une classe pouvant être une classe fille mais aussi une classe parent.  (cf. exemple ci-dessous)
Héritage multiple : L’héritage est le moyen de spécialiser une classe sans compromettre son code original. PHP autorise l’héritage multiple. Une classe pouvant être une classe fille mais aussi une classe parent.  (cf. figure 1)

````php

````
Dans l'exemple ci-dessus, la classe B hérite de la classe A. La classe C hérite de la classe B.

### Final

Evidemment l’héritage multiple a fonctionnellement des limites. On peut souhaiter interdire l’héritage afin de 
conserver une certaine intégrité du code. C’est possible si on place le mot clé final devant le nom de la classe. 
(cf. exemple ci-dessous)

````php

````

Dans l'exemple ci-dessus, on ne pourra pas créer de classes à partir de la classe C. L’héritage est interdit.

### Classe abstraite

une classe abstraite ne peut pas être instanciée. L’héritage devient alors le seul moyen pour exploiter ses propriétés et 
ses méthodes. Les classes filles pouvant alors être instanciées. (cf. exemples ci-dessous). 


Classe abstraite, mot-clé abstract
Dans l'exemple ci-dessus, la classe A est abstraite. Elle ne peut pas être instanciée. Le code ci-dessous montre que 
l’instanciation de la classe A provoque une erreur *PHP : Fatal Error, cannot instanciate abstract class A*

L’intérêt de la classe Abstraite est de fournir un code de base (une sorte de modèle) commun à un ensemble de classes. 
Mais ce code n’est pas complet pour pouvoir l’utiliser directement. L’héritage est donc la seule solution de développement.


Ci-dessus, application, classe abstraite, instanciation impossible.

### Accès statique

une classe peut posséder des propriétés statiques. Ces propriétés ne sont pas des propriétés liées aux objets, mais des 
propriétés de classe. Il est ainsi possible d’exploiter cette caractéristique pour connaître par exemple le nombre 
d’instances créées. Cela s’avère particulièrement utile lors de la mise en œuvre de l’héritage. Mais pas seulement. 
(cf. exemples ci-dessous)



Dans le code ci-dessus, il est possible de connaître le nombre d’instances (objets) créées. 

## Travail à faire

## CREATION DE CLASSES AVEC HERITAGE (voiture.PHP)

Voici la représentation UML du diagramme des classes à créer dans cet exercice.




###	Classe VehiculeAMoteur

Créer la classe Abstraite VehiculeAMoteur dont les caractéristiques sont les suivantes :

* Propriétés
    *	Type de moteur (propriété encapsulée)
    *	Nombre de passagers (propriété encapsulée)
    *	Nombre de véhicules (propriété de la classe : Static)
*	Méthodes
    *	Le constructeur
    *	verificationtype($type) : cette méthode permet de vérifier que l’utilisateur de la classe utilisera bien le bon code pour la propriété Type moteur. Il vaut soit T, soit E. (T pour Thermique, E pour Electrique)
    *	verificationnbpassagers($nombre) : cette méthode permet de vérifier que l’utilisateur de la classe affecte bien une valeur numérique (un entier) au nombre de passagers.

###	Classe Voiture

Créer la classe Voiture qui hérite de la classe VehiculeAMoteur  dont les caractéristiques sont les suivantes :

*	Propriétés
    *	Marque du véhicule
    *	Puissance en chevaux 
*	Méthodes
    *	Le constructeur
    *	Lirecaracteristiques() qui retourne :
        *	Le type de moteur,
        *	Le nombre de passagers
        *	La marque
        *	La puissance

###	Classe VoitureDeSport

Créer la classe VoitureDeSport qui hérite de la classe Voiture. Il ne doit pas être possible de créer des classes fillesà partir de la classe VoitureDeSport.

*	Propriété :
    *	Nb de secondes de zéro à  km/h
*	Méthodes :
    * Le constructeur 
    *	Lirecaracteristiques() héritée de la classe Voiture et qui affiche en plus le nombre de secondes de zéro à cent.

###	Classe VoitureTourisme

Créer la classe VoitureTourisme qui hérite de la classe Voiture dont les caractéristiques sont les suivantes :

* Propriétés :
    *	Consommation en litres pour 100 kilomètres.
    *	Kilométrage.
*	Méthodes :
    *	Le constructeur
    *	Lirecaracteristiques() héritée de la classe Voiture et qui retourne en plus la consommation et le kilométrage.
    *	utiliser($distance) : incrémente le kilometrage dun nombre de kilomètres donné en argument ($distance)

###	Classe Camion

Créer la classe Camion qui hérite de la classe VehiculeAMoteur dont les caractéristiques sont les suivantes :

*	Propriétés :
    *	Tonnage
    *	Nombre d’essieux
*	Méthodes
    *	Le constructeur
    *	lirecaracteristiques() qui retourne :
        *	Type moteur,
        *	Nombre de passagers
        *	Le tonnage
        *	Le nombre d’essieux 
    
##	CREATION DE L’APPLICATION (TD6.PHP)

Voici le code de l’application attendue. A saisir et à tester.



