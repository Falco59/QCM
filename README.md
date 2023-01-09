QCM Javascript
Jean-Philippe FUMIERE



Quelle est la syntaxe de base d’une déclaration de variable en JavaScript?

Voici la syntaxe de base d'une déclaration de variable en JavaScript : let nomDeVariable = valeur; ou var nomDeVariable = valeur;.

Quelle est la différence entre let et var en JavaScript?
let est une instruction de déclaration de variable introduite dans ECMAScript 6. Elle est similaire à var, mais elle a une portée de bloc (par exemple, entre accolades) au lieu de la portée de fonction. Cela signifie que la variable déclarée avec let n'est accessible que dans le bloc où elle a été déclarée. var, en revanche, a une portée de fonction et est accessible partout dans la fonction où elle a été déclarée.

Quelle est la différence entre null et undefined en JavaScript?
En JavaScript, null est un objet qui représente la valeur "aucune valeur". C'est un objet spécial qui est utilisé pour représenter l'absence de valeur. undefined, quant à lui, est une valeur primitive qui est utilisée pour indiquer qu'une variable a été déclarée, mais qu'elle n'a pas encore été initialisée ou qu'elle n'a pas de valeur.

Comment concaténer deux chaînes de caractères en JavaScript?
Pour concaténer deux chaînes de caractères en JavaScript, vous pouvez utiliser l'opérateur de concaténation (+) : let chaineConcatenee = chaine1 + chaine2;. Vous pouvez également utiliser la méthode concat() de l'objet String : let chaineConcatenee = chaine1.concat(chaine2);.

Comment convertir une chaîne en entier en JavaScript?
Pour convertir une chaîne en entier en JavaScript, vous pouvez utiliser la fonction parseInt() : let entier = parseInt(chaine);. Si la chaîne ne peut pas être convertie en entier, parseInt() renverra NaN (Not a Number).
Comment créer une fonction en JavaScript?
function nomDeFonction(parametres) {
  // instructions
}

Quelle est la différence entre une fonction déclarative et une fonction exprimée en JavaScript?
Une fonction déclarative est une fonction qui est déclarée au début de la portée (généralement au niveau global ou au niveau de la fonction) avec le mot-clé function. Une fonction exprimée, en revanche, est une fonction qui est créée en assignant une fonction à une variable. Voici un exemple de fonction exprimée :
Copy code
let maFonction = function(parametres) {
  // instructions
}


// Ok mais c'est du copié collé. 


Comment appeler une fonction en JavaScript?
Pour appeler une fonction en JavaScript, vous devez utiliser son nom suivi de parenthèses et éventuellement de arguments entre parenthèses : nomDeFonction(arguments);.

Comment passer des arguments à une fonction en JavaScript?

Pour passer des arguments à une fonction en JavaScript, vous devez les fournir entre parenthèses lors de l'appel de la fonction, séparés par des virgules s'il y en a plusieurs. Par exemple : maFonction(arg1, arg2, arg3);. Ces arguments seront alors disponibles à l'intérieur de la fonction sous forme de variables avec les noms spécifiés dans la déclaration de la fonction (par exemple, parametres dans l'exemple de code précédent).

Comment utiliser une boucle for en JavaScript?

Voici comment utiliser une boucle for en JavaScript :

Copy code
for (initialisation; condition; incrementation) {
  // instructions à exécuter tant que la condition est vraie
}
La boucle for commence par l'initialisation de la boucle (par exemple, la déclaration et l'initialisation d'une variable de boucle). Ensuite, la condition est vérifiée. Si elle est vraie, les instructions de la boucle sont exécutées. Enfin, l'incrementation (ou décrementation) est effectuée et la boucle revient au début en vérifiant à nouveau la condition. Si la condition est toujours vraie, les instructions sont à nouveau exécutées, et ainsi de suite. Si la condition devient fausse, la boucle s'arrête.
Voici un exemple de boucle for qui affiche les nombres de 1 à 10 :
Copy code
for (let i = 1; i <= 10; i++) {
  console.log(i);
}
Comment utiliser une boucle while en JavaScript?
Voici comment utiliser une boucle while en JavaScript :

Copy code
while (condition) {
  // instructions à exécuter tant que la condition est vraie
}
La boucle while vérifie d'abord la condition. Si elle est vraie, les instructions de la boucle sont exécutées. Ensuite, la condition est à nouveau vérifiée, et ainsi de suite jusqu'à ce qu'elle devienne fausse. Si la condition est fausse au départ, les instructions de la boucle ne sont pas exécutées du tout.

Comment utiliser une boucle do...while en JavaScript?
Pour utiliser une boucle do...while en JavaScript, vous pouvez écrire quelque chose comme ceci :

Copy code
do {
  // code à exécuter
  // ...
} while (condition);
La boucle do...while exécute d'abord le code à l'intérieur des accolades {}, puis vérifie si la condition est vraie. Si la condition est vraie, la boucle est exécutée de nouveau. Si la condition est fausse, la boucle s'arrête.
Il est important de noter que la boucle do...while sera au moins exécutée une fois, même si la condition est fausse dès le départ. Cela la distingue de la boucle while, qui ne sera pas exécutée du tout si la condition est fausse dès le départ.

Comment utiliser l’instruction break dans une boucle en JavaScript?
L'instruction break permet de sortir d'une boucle en JavaScript avant que la condition de fin de boucle ne soit atteinte. Elle est souvent utilisée pour mettre fin à une boucle lorsque certaines conditions sont remplies.

Voici comment utiliser break dans une boucle for :

Copy code
for (let i = 0; i < 10; i++) {
  if (i === 5) {
    break;
  }
  console.log(i);
}
Ce code affichera les nombres de 0 à 4 dans la console, puis sortira de la boucle lorsque i sera égal à 5. La boucle ne sera pas exécutée pour les valeurs de i supérieures à 5.

Comment utiliser l’instruction continue dans une boucle en JavaScript?
L'instruction continue en JavaScript permet de forcer l'interruption de l'itération en cours d'une boucle et de passer à la prochaine itération. Voici un exemple de boucle for qui utilise continue :

Copy code
for (let i = 0; i < 10; i++) {
  if (i === 5) {
    continue;
  }
  console.log(i);
}
Ce code affichera les nombres de 0 à 4 et de 6 à 9, car lorsque i vaut 5, l'instruction continue est exécutée et l'itération en cours est interrompue, passant directement à la prochaine itération de la boucle.

Vous pouvez également utiliser continue avec une étiquette pour interrompre une itération dans une boucle imbriquée. Par exemple :

Copy code
outerLoop: for (let i = 0; i < 10; i++) {
  for (let j = 0; j < 10; j++) {
    if (j === 5) {
      continue outerLoop;
    }
    console.log(i, j);
  }
}
Dans ce cas, l'instruction continue outerLoop interrompra l'itération en cours de la boucle outerLoop lorsque j vaut 5, passant directement à la prochaine itération de outerLoop.

Quelle est la différence entre l’opérateur == et l’opérateur === en JavaScript ?

En JavaScript, l'opérateur == (égal à) permet de vérifier si deux valeurs sont égales en effectuant une conversion de type si nécessaire. Par exemple :

Copy code
console.log(1 == '1'); // affiche true
Dans ce cas, le nombre 1 et la chaîne de caractères '1' sont considérés comme égaux, car JavaScript a converti la chaîne en nombre avant de faire la comparaison.

L'opérateur === (strictement égal à) est quant à lui plus strict et ne effectue pas de conversion de type. Il vérifie si deux valeurs sont égales en comparant leur type et leur valeur. Par exemple :

Copy code
console.log(1 === '1'); // affiche false
Dans ce cas, le nombre 1 et la chaîne de caractères '1' ne sont pas considérés comme égaux, car ils ont des types différents (un nombre et une chaîne de caractères).

En général, il est recommandé d'utiliser l'opérateur === lorsque vous faites des comparaisons en JavaScript, car il est plus strict et moins sujet aux erreurs. Cependant, il peut être utile d'utiliser l'opérateur == dans certains cas, comme lorsque vous voulez ignorer la différence entre null et undefined.


Comment utiliser un opérateur ternaire en JavaScript ?
La bonne façon de l'utiliser c'est de l'utiliser pour ce qu'il est c'est à dire un opérateur et d'exploiter sa valeur de retour. Vous pouvez le faire dans une affectation. Vous en avez un exemple ci-dessous : si la condition est vraie alors la valeur 1 est affectée à x sinon c'est la valeur 0.

Comment créer un tableau en JavaScript ?
Déclaration de base
Un tableau est un objet Array. Pour déclarer un tableau, il faut utiliser l'instruction new :
var tab=new Array();
La variable tab a maintenant la structure d'un tableau. Elle possède les propriétés et les méthodes des tableaux et est prête à recevoir le contenu du tableau.
En JavaScript, comme dans la plupart des langages de programmation, le premier élément du tableau commence à l'indice 0. C'est un peu gênant, mais on s'habitue...
Pour alimenter le tableau avec les jours de la semaine, on écrit le code suivant :
var tab=new Array();
tab[0]="Lundi";
tab[1]="Mardi";
tab[2]="Mercredi";
tab[3]="Jeudi";
tab[4]="Vendredi";
tab[5]="Samedi";
tab[6]="Dimanche";
var longueur=tab.length;

Comment accéder à un élément d’un tableau en JavaScript?
Accéder aux éléments d'un tableau
let arr = ["le premier élément", "le deuxième élément", "le dernier élément"]; console. log(arr[0]); // affiche "le premier élément" console. ...
let années = [1950, 1960, 1970, 1980, 1990, 2000, 2010]; console. log(années. ...
renderer. 3d.

Comment utiliser la méthode push pour ajouter un élément à la fin d’un tableau en JavaScript?
Pour ajouter une valeur à un tableau, il suffit de faire appel à la méthode push(). Cette méthode retourne la longueur du tableau une fois les nouvelles valeurs ajoutées.

var monTableau = [x, y, z];
var longueur = monTableau.push(a);
console.log(monTableau); //Cette commande affichera [x, y, z, a]
console.log(longueur); //Cette commande affichera 4

Comment utiliser la méthode pop pour supprimer un élément de la fin d’un tableau en JavaScript?
La méthode pop() est une méthode de l'objet Array qui permet de supprimer le dernier élément d'un tableau et de renvoyer cet élément. Voici comment l'utiliser :

Copy code
let tableau = [1, 2, 3, 4, 5];

let dernierElement = tableau.pop();

console.log(dernierElement); // affiche 5
console.log(tableau); // affiche [1, 2, 3, 4]
Si vous voulez supprimer le premier élément du tableau, vous pouvez utiliser la méthode shift(), qui fonctionne de la même manière que pop(), mais en supprimant le premier élément au lieu du dernier.

Copy code
let tableau = [1, 2, 3, 4, 5];

let premierElement = tableau.shift();

console.log(premierElement); // affiche 1
console.log(tableau); // affiche [2, 3, 4, 5]

Comment utiliser la méthode shift pour supprimer un élément du début d’un tableau en JavaScript?
La méthode shift() est une méthode de l'objet Array qui permet de supprimer le premier élément d'un tableau et de renvoyer cet élément. Voici comment l'utiliser :

Copy code
let tableau = [1, 2, 3, 4, 5];

let premierElement = tableau.shift();

console.log(premierElement); // affiche 1
console.log(tableau); // affiche [2, 3, 4, 5]
Si vous voulez supprimer le dernier élément du tableau, vous pouvez utiliser la méthode pop(), qui fonctionne de la même manière que shift(), mais en supprimant le dernier élément au lieu du premier.

Copy code
let tableau = [1, 2, 3, 4, 5];

let dernierElement = tableau.pop();

console.log(dernierElement); // affiche 5
console.log(tableau); // affiche [1, 2, 3, 4]

Comment utiliser la méthode unshift pour ajouter un élément au début d’un tableau en JavaScript?

var langages = ["JavaScript", "HTML", "CSS"];
langages. unshift("PHP");
console. log(langages);
langages. unshift("Java", "Python");
console. log(langages);
for(var i = 0; i < langages. length; i++){
write("" + langages[i] + "");

Comment utiliser la méthode splice pour ajouter, supprimer ou remplacer des éléments d’un tableau en JavaScript?
La méthode splice() est une méthode de l'objet Array qui permet d'ajouter, de supprimer ou de remplacer des éléments d'un tableau. Voici comment l'utiliser :

Copy code
let tableau = [1, 2, 3, 4, 5];

// pour ajouter un élément
tableau.splice(2, 0, 'a', 'b');
console.log(tableau); // affiche [1, 2, "a", "b", 3, 4, 5]

// pour remplacer un élément
tableau.splice(2, 1, 'c');
console.log(tableau); // affiche [1, 2, "c", "b", 3, 4, 5]

// pour supprimer un élément
tableau.splice(2, 1);
console.log(tableau); // affiche [1, 2, "b", 3, 4, 5]

// pour remplacer plusieurs éléments
tableau.splice(2, 3, 'd', 'e', 'f');
console.log(tableau); // affiche [1, 2, "d", "e", "f"]
La méthode splice() prend deux arguments obligatoires :

l'index à partir duquel les éléments doivent être ajoutés, supprimés ou remplacés
le nombre d'éléments à supprimer (si vous voulez ajouter ou remplacer des éléments, mettez 0)
Vous pouvez également lui passer d'autres arguments optionnels, qui représentent les valeurs à ajouter ou à remplacer.

La méthode splice() modifie le tableau original et renvoie un tableau contenant les éléments qui ont été supprimés. Si vous ne supprimez aucun élément, elle renvoie un tableau vide.

Comment utiliser la méthode slice pour copier un sous - tableau d’un tableau en JavaScript?
Array.prototype.slice()
La méthode slice() renvoie un objet tableau, contenant une copie superficielle (shallow copy) d'une portion du tableau d'origine, la portion est définie par un indice de début et un indice de fin (exclus). Le tableau original ne sera pas modifié.

Comment parcourir un tableau en JavaScript avec la méthode forEach ?
La méthode forEach() transmet une boucle de rappel (callback) à chaque éléments du tableau avec les paramètres suivants:
La valeur actuelle (obligatoire) - La valeur de l'élément actuel du tableau.
L'index (facultatif) - L'index de l'élément actuel.
Array (facultatif) - L'objet tableau d'origine des éléments concernés.

Comment utiliser la méthode map pour transformer chaque élément d’un tableau en JavaScript?
Array.prototype.map()
La méthode map() crée un nouveau tableau avec les résultats de l'appel d'une fonction fournie sur chaque élément du tableau appelant.

Comment utiliser la méthode filter pour filtrer les éléments d’un tableau en JavaScript?
La méthode filter() est une méthode de l'objet Array qui permet de filtrer les éléments d'un tableau en fonction d'une condition donnée. Elle renvoie un nouveau tableau contenant uniquement les éléments qui satisfont cette condition.

Voici comment l'utiliser :

Copy code
let tableau = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

let resultat = tableau.filter(function(element) {
  return element % 2 == 0;
});

console.log(resultat); // affiche [2, 4, 6, 8, 10]
La fonction de filtrage prend chaque élément du tableau en argument et doit renvoyer true si l'élément doit être inclus dans le nouveau tableau, ou false s'il doit être ignoré. Dans l'exemple ci-dessus, la fonction vérifie si l'élément est un nombre pair, et ne garde que les éléments qui le sont.

Vous pouvez également utiliser une fonction fléchée au lieu d'une fonction traditionnelle :

Copy code
let resultat = tableau.filter(element => element % 2 == 0);
Notez que la méthode filter() ne modifie pas le tableau original, elle renvoie un nouveau tableau. Si vous voulez modifier le tableau original, vous pouvez utiliser la méthode splice() :

Copy code
let i = 0;
while (i < tableau.length) {
  if (tableau[i] % 2 != 0) {
    tableau.splice(i, 1);
  } else {
    i++;
  }
}

console.log(tableau); // affiche [2, 4, 6, 8, 10]
Cette boucle parcourt le tableau et supprime chaque élément qui n'est pas un nombre pair en utilisant splice(). Le compteur i est incrémenté seulement si l'élément est gardé, afin de ne pas sauter un élément lors de la suppression.

Comment utiliser la méthode reduce pour réduire un tableau en une valeur unique en JavaScript ?
Array.prototype.reduce()
La méthode reduce() applique une fonction qui est un « accumulateur » et qui traite chaque valeur d'une liste (de la gauche vers la droite) afin de la réduire à une seule valeur.

Comment créer un objet en JavaScript ?
Il existe plusieurs manières de créer un objet en JavaScript. Voici quelques exemples :

En utilisant une syntaxe de littéral d'objet :
Copy code
let objet = {
  propriete1: valeur1,
  propriete2: valeur2,
  ...
};
Par exemple :

Copy code
let personne = {
  nom: 'Dupont',
  prenom: 'Jean',
  age: 30
};

console.log(personne.nom); // affiche 'Dupont'
console.log(personne.prenom); // affiche 'Jean'
console.log(personne.age); // affiche 30
En utilisant le constructeur Object() :
Copy code
let objet = new Object();
objet.propriete1 = valeur1;
objet.propriete2 = valeur2;
...
Par exemple :

Copy code
let personne = new Object();
personne.nom = 'Dupont';
personne.prenom = 'Jean';
personne.age = 30;

console.log(personne.nom); // affiche 'Dupont'
console.log(personne.prenom); // affiche 'Jean'
console.log(personne.age); // affiche 30

Comment accéder à une propriété d’un objet en JavaScript ?
Indexer les propriétés d'un objet
Il est possible d'accéder à une propriété via son nom et via son indice (ordinal). Si on définit une propriété grâce à un nom, on accédera toujours à la valeur via le nom. De même, si on définit une propriété grâce à un indice, on y accèdera toujours via son indice.

Cette restriction s'applique lorsqu'on crée un objet et ses propriétés via un constructeur et lorsqu'on déclare les propriétés explicitement (par exemple avec maVoiture.couleur = "rouge"). Si on définit une propriété d'un objet avec maVoiture[5] = "25 kmh", on pourra faire référence à cette propriété grâce à maVoiture[5].

Il existe une exception à cette règle lorsqu'on manipule des objets "semblables à des tableaux" provenant d'API Web telles que l'objet forms. Pour ces objets semblables à des tableaux, on peut accéder à une propriété de l'objet grâce à son nom (si l'attribut name est utilisé sur l'élément HTML) ou grâce à son index selon l'ordre dans le document. Ainsi, si on souhaite cibler un élément <form> du document possédant un attribut name qui vaut monForm et que cet élément est le deuxième élément du document, on pourra y accéder avec document.forms[1], document.forms["monForm"] ou encore avec document.forms.monForm.

Définir des propriétés pour un type d'objet
On peut ajouter une propriété à un type précédemment défini en utilisant la propriété prototype. Cela permettra de définir une propriété qui sera partagée par tous les objets d'un même type plutôt qu'elle ne soit définie que pour un seul objet. Le code suivant permet d'ajouter une propriété couleur à tous les objets de type voiture. On affecte ensuite une valeur à cette propriété pour l'objet voiture1.

Voiture.prototype.couleur = null;
voiture1.couleur = "noir";

Comment définir une propriété d’un objet en JavaScript ?
Définir des propriétés pour un type d'objet
On peut ajouter une propriété à un type précédemment défini en utilisant la propriété prototype . Cela permettra de définir une propriété qui sera partagée par tous les objets d'un même type plutôt qu'elle ne soit définie que pour un seul objet.

Comment supprimer une propriété d’un objet en JavaScript ?
La méthode Reflect. deleteProperty permet de supprimer une propriété d'un objet. Elle renvoie un Boolean qui indique si la propriété a été supprimée correctement. Cette méthode est très proche de l'opérateur delete

quelle différence entre java et javascript ?

Java permet de créer des applications qui sont exécutées sur une machine ou un navigateur virtuel tandis que le code JavaScript est exécuté uniquement sur un navigateur. Le code Java doit être compilé tandis que le code JavaScript est composé entièrement de texte. Ils nécessitent des plug-ins différents.
