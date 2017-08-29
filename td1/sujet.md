## TD1 : Révisions du PHP

Ce TD a pour objectif de faire un rappel sur les notions de tableau et de fonction en PHP :
* Certains exercices nécessiteront l’utilisation de tableaux pour rendre la POO plus concrète.
* En POO, une méthode est une fonction. Il est donc important de maîtriser leur mise en oeuvre.

### Les tableaux

Le but de ces exercices est de faire un rappel rapide de la notion de tableau, qu’il soit en une ou deux dimensions.

#### Tableau 1 dimension

* Saisissez ce code. Nommez le fichier td1_tableau.php
* Testez-le

#### Tableau associatif

* Saisissez ce code. Nommez le fichier td1_tableau_associatif.php
* Testez-le

#### Tableau 2 dimensions

* Saisissez ce code. Nommez le fichier td1_tableau_2d.php
* Testez-le

### Les fonctions

#### Quelques rappels pour commencer...

* Intérêt d’une fonction : Dans un code lorsque des instructions se répètent, il est judicieux de créer une
fonction qui les regroupera dans un bloc. L’exécution de ces instructions se résumera à l’appel de la
fonction. Le code en sera simplifié et la maintenance plus aisée.
* Paramètre : Une fonction peut avoir ou non en entrée des paramètres (on dit aussi arguments). Ainsi les
instructions exécutées dans la fonction vont pouvoir traiter les valeurs fournies en paramètres et donner
des résultats différents. Les paramètres peuvent être des variables (nombre, texte, date, tableau, …) ou
des constantes.
* Variable locale : Le bloc fonction peut utiliser ses propres variables. Ces variables sont dites locales. C’est-
à-dire que celles-ci n’existeront que lorsque la fonction sera appelée.
* Notion de valeur de retour : Une fonction peut posséder ou non une valeur de retour. Ainsi le code
principal de l’application pourra récupérer le résultat de la fonction.

  > Bibliographie :
  [Claude DELANNOY] - « S’initier à la programmation et à l’orienté objet » - Edition EYROLLES – Pages 163–171
  
#### Mise en œuvre en PHP

On vous fournit le code suivant.

1. Saisissez ce code. Nommez le fichier nommé td1_fonction.php puis testez-le
2. Modifiez le code pour :

* Créez une fonction footer
1. Elle possède 3 arguments : le nom de l’IUT, le département et le nom du module
2. Elle retourne une chaine de caractères qui la concaténation des 3 arguments
* Ajoutez le code qui appellera la fonction footer et affichera la valeur qu’elle retourne.

3. Comparez les deux fonctions affichage_footer et footer.
