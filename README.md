# JAVA cours

## Variables

>Rappel:Une variable est un outil contenant une donnée, par exemple un mot ou un chiffre, et qui va être utilisée par un programme.Un programme manipule constamment des variables, soit que l'on a définies, soit qu'il a créées.Les variables contiennent des **valeurs**, ces variables sont gérées et enregistrées par l'ordinateur. Pour savoir ce qu'elles contiennent nous leurs donons un nom.

### Les nommer

Son nom doit reflèter son contenu.

Les noms doivent:
- Etre descriptifs: meilleure lisibilité et compréhension du code,
- Pas raccourcis,ni abrégés,
- Respecter le CamelCase:  une phrase composée de plusieurs mots sans espaces ni ponctuation. Le premier mot est écrit en minuscules et tous les autres mots commencent par une majuscule,

## Les déclarer

Pour utiliser les variables, il faut les créer, ou **déclarer**.
>Il existe plusieurs types de variables, en fonction du type de valeur qu'elles contiennent.

En Java, par exemple, si la variable contient un nombre entier elle sera déclarée en utilisant le mot clé **int** suivi du nom de la variable? On dit que ce sont des **ints**.

Exemple:

    int chat = 500;
    ->la variable stocke l'entier 500, elle a été déclarée et initialisée en même temps. (Assignation d'une valeur de départ)

En Java, chaque instruction se termine par un **;**

Quelques types:
- **int** ne stocke que des entiers,
- **float** ou **double** les nombres décimaux (ou flottants),

### Modifier les valeurs des variables avec les opérateurs

Une variable peut varier c'est à dire chageer de valeur.
Elle peut varier grâce à des **opérateurs**.

>Les règles arithmétiques s'appliquent! L'on utilise les () pour décider des opérations prioritaires.

|Opérateur|Usage|
|-----------:|---------:|
|+|addition|
|-|soustraction|
|*|multiplication|
|/|division|

Exemple:

    public class ManipulationVariables {
        public static void main(String[] args) {
            int epargne = 500;
            int revenus = 2000;
            //Ajoutez 100 à votre épargne (Yeah!)
            epargne = epargne + 100;

            //Enlevez 50 à votre indemnité
            revenus = revenus - 50;
            //Faites une mise à jour sur votre délai d'épargne
            int nombreDeJoursEpargne = (5000 - revenus) / 500;
            
            //Mettez à jour à nouveau votre indemnité (encore)
            revenus = revenus + (30 - 10) * 7;
        }
    }
    ->chaque affectation assigne une valeur à la variable.
Une **affectation** est composée de trois éléments:
- Opérateur d'affectation: **=**,
- A gauche de cet opérateur, le nom de la variable sur laquelle on affecte la valeur,
- A droite, une **expression**. Une expression, est une affectation qui produit une valeur.
  
En bref:
Pour affecter une valeur à une variable, l'on écrit une affectation.
Elle se compose du nom de la variable, suivi de l'opérateur d' affectation, et ensuite de l' expression qui produit une valeur correspondant au type de la variable.

#### Ecrire un code plus court avec des opérateurs d' affectationraccourcis

Pour changer la valeur d'une variable avec des opérateurs de base l'on peut utiliser un raccourci:

    epargne = epargne + 100;
    =>
    epargne += 100;

Cela fonctionne donc avec:
-=
*=
/=

### Manipuler d' autres données que les nombres

Pour stocker différents contenus dans les variables, l' on doit définier le type de celle-ci.
En effet, en fonction du type, les variables stockées dans la mémoire de l'ordinateur ne prennent pas la même place.

Il existe les variables:
- texte: **String**,
- entier: **int**,
- float: **double**.
  
Exemple de déclaration de variables:

    String text = "blabla";
    int numberOfCat = 10;
    double percentage = 0.0;

### Les variables qui ne " changent pas"

Ceratines valeurs n'ont pas besoin d' être modifiées. Elles restent telles qu' elles étaient au début;
Ce sont des **constantes**.
Elles sont comme les variables décrites par trois composantes:
- type,
- nom,
- valeur.

Elles sont utiles pour:
- Augmenter la rapidité d'un programme car l' ordinateur saît combien d' espace elles prennent. Ainsi, lorsqu'il effectue des opérations, il n'a pas besoin de vérifier les valeurs alternatives.
- S'assurer que certaines valeurs ne changent pas notamment par mégarde.

**A utiliser dans la mesure du possible !**

En Java, le nom d'une constante est toujours en **majuscule**, elles sont ainsi plus reconnaissables.
Elles sont déclarées grâce au mot clé **final**.

Exemples:

    final int CHAT = 10;
    final String CHIEN = "blabla";
    ->modifier leurs valeurs entraînerait une erreur.

### Spécifier le bon type de variable

La seule façon de déclarer une variable en Java est de spécifier directement son type.

Exemple:

    int count = 10;
    int: type,
    count: nom,
    10: valeur.
**Même si l'on a pas de valeur à assigner au départ, il faut utiliser le mot clé du type.**

Exemple:

    int chat;
    ->déclaration sans valeur.
Dans ce cas, l'on ne peut l'utiliser sans lui avoir attribuer une valeur! Il faudra lui assigner par la suite.
Déclarer sans valeur mais avec le type, permet au processeur de lui allouer un espace mémoire.

>Parmi les types de données, il existe les types primitifs: ils existent par eux-mêmes. Exemples: int et double. L'on peut les combiner pour en faire des plus complexes. Dans les types primitifs, il existe notamment: **les types numériques** et **les chaînes**.

### Les types numériques







## Sources
[open classroom](https://openclassrooms.com/fr/courses/6173501-apprenez-a-programmer-en-java/6313896-declarez-des-variables)