# JAVA cours

![Logo Java](img/Java_Logo.svg.png)

## Simplon

### Généralités


Java est:

**Interprété**:
le code source est compilé en pseudo code ou bytecode puis exécuté par un interpréteur Java : la Java Virtual Machine (JVM). Ce concept est à la base du slogan de Sun pour Java : WORA (Write Once, Run Anywhere : écrire une fois, exécuter partout). En effet, le bytecode, s'il ne contient pas de code spécifique à une plate-forme particulière peut être exécuté et obtenir quasiment les mêmes résultats sur toutes les machines disposant d'une JVM.

**Portable**: 
il n'y a pas de compilation spécifique pour chaque plate forme. Le code reste indépendant de la machine sur laquelle il s'exécute. Il est possible d'exécuter des programmes Java sur tous les environnements qui possèdent une Java Virtual Machine. Cette indépendance est assurée au niveau du code source grâce à Unicode et au niveau du bytecode.
**Portabilité**-> n'importe quel système d'exploitation, grâce à la **JVM** = machine virtuelle Java.
Traduit le code Java en code binaire.

**Orienté objet**:
comme la plupart des langages récents, Java est orienté objet. Chaque fichier source contient la définition d'une ou plusieurs classes qui sont utilisées les unes avec les autres pour former une application. Java n'est pas complètement objet car il définit des types primitifs (entier, caractère, flottant, booléen,...).

**Fortement typé**:
toutes les variables sont typées et il n'existe pas de conversion automatique qui risquerait une perte de données. Si une telle conversion doit être réalisée, le développeur doit obligatoirement utiliser un cast ou une méthode statique fournie en standard pour la réaliser.

**Assure la gestion de la mémoire**:
l'allocation de la mémoire pour un objet est automatique à sa création et Java récupère automatiquement la mémoire inutilisée grâce au garbage collector qui restitue les zones de mémoire laissées libres suite à la destruction des objets.

**Sûr**:
la sécurité fait partie intégrante du système d'exécution et du compilateur. Un programme Java planté ne menace pas le système d'exploitation. Il ne peut pas y avoir d'accès direct à la mémoire. L'accès au disque dur est réglementé dans une applet.
Les applets fonctionnant sur le Web sont soumises aux restrictions suivantes dans la version 1.0 de Java :
aucun programme ne peut ouvrir, lire, écrire ou effacer un fichier sur le système de l'utilisateur
aucun programme ne peut lancer un autre programme sur le système de l'utilisateur
toute fenêtre créée par le programme est clairement identifiée comme étant une fenêtre Java, ce qui interdit par exemple la création d'une fausse fenêtre demandant un mot de passe
les programmes ne peuvent pas se connecter à d'autres sites Web que celui dont ils proviennent.

**POO = Programmation Orienté Objet**.

>*Lorsqu’un programmeur écrit une application Java, le code compilé (appelé bytecode) s’exécute sur la plupart des systèmes d’exploitation (OS), y compris Windows, Linux et Mac OS. Java tire une grande partie de sa syntaxe des langages de programmation C et C++. La plate-forme Java (l’environnement dans lequel un programme s’exécute) se distingue du fait qu’elle s’exécute sur d’autres plateformes matérielles. Elle comporte deux composants : la machine virtuelle Java (Java VM) et l’interface de programmation d’applications Java (API Java).Java a été développée au milieu des années 1990 par James A. Gosling, un ancien informaticien de Sun Microsystems, avec Mike Sheridan et Patrick Naughton.Tous les programmes sont constitués d’entités représentant des concepts ou des choses physiques appelées « objets ». Les programmes Java se trouvent dans les ordinateurs de bureau, les serveurs, les appareils mobiles, les cartes à puce et les disques Blu-ray (BD). Le développement de programmes Java nécessite un kit de développement logiciel Java (SDK), qui comprend généralement un compilateur, un interpréteur, un générateur de documentation et d’autres outils utilisés pour produire une application complète.Le temps de développement peut être accéléré grâce à l’utilisation d’environnements de développement intégrés (IDE) – tels que JBuilder, Netbeans, Eclipse ou JCreator. Les IDE facilitent le développement d’interfaces graphiques, qui incluent des boutons, des zones de texte, des panneaux, des cadres, des barres de défilement et d’autres objets via des actions de glisser-déposer et de pointer-cliquer.*

>*La plate-forme Java est indépendante et peut fonctionner sur tous les systèmes d’exploitation disponibles en ce qui concerne son développement et sa compilation. Cela est possible du fait du bytecode, un code qui est compréhensible par la machine. La plateforme se compose du langage Java, du kit de développement Java (JDK), de l’environnement d’exécution Java (JRE), du compilateur Java et de la « Java Virtual Machine » (JVM).*

Il existe 2 types de programmes avec la version standard de Java : **les applets et les applications**. Une application autonome (stand alone program) est une application qui s'exécute sous le contrôle direct du système d'exploitation. Une applet est une application qui est chargée par un navigateur et qui est exécutée sous le contrôle d'un plug in de ce dernier.

Les principales différences entre une applet et une application sont :
les applets n'ont pas de méthode main() : la méthode main() est appelée par la machine virtuelle pour exécuter une application.
les applets ne peuvent pas être testées avec l'interpréteur. Elles doivent être testées avec l'applet viewer ou doivent être intégrées à une page HTML, elle même visualisée avec un navigateur disposant d'un plug in Java, .


#### Notes

*Oracle a racheté Java et en ont fait une licence GNU, semi-opensource.*

JSE, JEE, JSK, ...
Java Standard Edition, Java Enterprice Edition, Java Software Kit, ...

**IoT**: internet des objets, utilisés au quotidien. 
Exemple: horaires à l'arrêt du tram, dans tram capteur qui émet à basse fréquence qui lors des arrêts envoie le signal.

### Installation

Voit dossier TestJava.

- **JSE**: environnement d'exécution standard de Java, outils, bibliothèques...  Java Standard Edition.
- **JDK**: ensemble d'outils nécessaires au développement (regroupe le JSE et outils de compilation (**javac**), JRE, outil de création jar: extension .jar = ). Pour les développeurs. Java Development Kit.
Le JDK de Sun/Oracle fournit un ensemble d'outils qui permettent de réaliser des applications. Ces outils sont peu ergonomiques car ils s'utilisent en ligne de commandes mais, en contrepartie, ils peuvent toujours être utilisés.
- **JRE**: plateforme Java, Java Runtime Envirronement, environnement d'exécution. Pour les user d'application, sans les développer.

>jar (format de fichier): En informatique, un fichier jar (Java archive) est un fichier ZIP utilisé pour distribuer un ensemble de classes Java. Ce format est utilisé pour stocker les définitions des classes, ainsi que des métadonnées, constituant l'ensemble d'un programme.

[Java SE](https://www.oracle.com/fr/java/) ->
JDK Development Kit 20.0.1 downloads: 	
https://download.oracle.com/java/20/latest/jdk-20_windows-x64_bin.exe (sha256)

>Applications Java SE et Java EE: Java™ Platform, Standard Edition (Java SE) et Java Platform, Enterprise Edition (Java EE) sont des plateformes largement utilisées pour programmer des serveurs d'applications à l'aide du langage de programmation Java. Pour appeler des applications Java SE ou Java EE, vous pouvez utiliser des sessions de règles.

![Installation JDK Path variables enviromment](img/1-installation_JDK.PNG)
![Installation JDK Path variables enviromment](img/2-bin_JDK.PNG)
![Installation JDK Path variables enviromment](img/3-javac_JDK.PNG)
![Installation JDK Path variables enviromment](img/4-path_javac.png)
![Installation JDK Path variables enviromment](img/5-path.png)

Variables environnement: 
chemin javac, dans variables système, path. **Penser à ajouter après bin\javac.exe**.

Dans commande (wndows r):
javac.exe
java - version

#### Compilation  et exécution

Un programme Java est composé d'un ou plus généralement plusieurs fichiers source. N'importe quel éditeur de texte peut être utilisé pour éditer un fichier source Java.
Ces fichiers source possèdent l'extension .java. Ils peuvent contenir une ou plusieurs classes ou interfaces mais il ne peut y avoir qu'une seule classe ou interface déclarée publique par fichier. Le nom de ce fichier source doit obligatoirement correspondre à la casse près au nom de cette entité publique suivi de l'extension .java
Il est nécessaire de compiler le source pour le transformer en J-code ou bytecode Java qui sera lui exécuté par la machine virtuelle. Pour être compilé, le programme doit être enregistré au format de caractères Unicode : une conversion automatique est faite par le JDK si nécessaire.

Un compilateur Java, par exemple l'outil javac fourni avec le JDK est utilisé pour compiler chaque fichier source en fichier de classe possédant l'extension .class. Cette compilation génère pour chaque fichier source un ou plusieurs fichiers .class qui contiennent du bytecode.

Test.java -> javac Test.java -> Test.class (voir outils du JDK)

**Pour exécuter une application, la classe servant de point d'entrée doit obligatoirement contenir une méthode ayant la signature public static void main(String[] args). Il est alors possible de fournir cette classe à la JVM qui va charger le ou les fichiers .class utiles à l'application et exécuter le code**.

#### Les packages

Les fichiers sources peuvent être organisés en packages. Les packages définissent une hiérarchie de noms, chaque nom étant séparé par le caractère point. Le nom d'un package est lié à une arborescence de sous-répertoires correspondant à ce nom.

Ceci permet de structurer les sources d'une application car une application peut rapidement contenir plusieurs centaines voire milliers de fichiers source. Les packages permettent aussi d'assurer l'unicité d'une classe grâce à son nom pleinement qualifié (nom du package suivi du caractère «.» suivi du nom de la classe).


#### Les outils du JDK

##### Le compilateur javac

Cet outil est le **compilateur** : il utilise un fichier source Java fourni en paramètre pour créer un ou plusieurs fichiers contenant le **bytecode** Java correspondant. Pour chaque fichier source, un fichier portant le même nom avec l'**extension .class** est créé si la compilation se déroule bien. Il est possible qu'un ou plusieurs autres fichiers .class soient générés lors de la compilation de la classe si celle-ci contient des classes internes. Dans ce cas, le nom du fichier des classes internes est de la forme classe$classe_interne.class. Un fichier .class supplémentaire est créé pour chaque classe interne. 

Pour compiler tous les fichiers sources du répertoire:
javac *.java.

Pour compiler un fichier:
saisie de javac ./fichier.java pour compiler le code.

[développons en Java](https://www.jmdoudoux.fr/java/dej/chap-outils-jdk.htm) => erreur, sources, lignes de commande.

##### L'interpréteur Java

Ces deux outils sont les interpréteurs de bytecode : ils lancent le JRE, chargent les classes nécessaires et exécutent la méthode main de la classe passée en paramètre.

java fichier.java

##### L'outil jar

JAR est le diminutif de Java ARchive. C'est un format de fichier qui permet de regrouper des fichiers contenant du bytecode Java (fichier .class) ou des données utilisées en tant que ressources (images, son, ...). Ce format est compatible avec le format ZIP : les fichiers contenus dans un jar sont compressés de façon indépendante du système d'exploitation.

###### Lintérêt du format jar

Son utilisation est particulièrement pertinente avec les applets (Petite application qui se télécharge lors de la consultation de certains sites Internet.), les beans et même les applications. En fait, le format jar est le format de diffusion des composants Java.

Les fichiers jar sont compressés par défaut ce qui est particulièrement intéressant quelque soit leurs utilisations.

Pour une applet, le browser n'effectue plus qu'une requête pour obtenir l'applet et ses ressources au lieu de plusieurs pour obtenir tous les fichiers nécessaires (fichiers .class, images, sons ...).

Un jar peut être signé ce qui permet d'assouplir et d'élargir le modèle de sécurité, notamment celui des applets qui ont des droits restreints par défaut.

Les beans doivent obligatoirement être diffusés sous ce format.

Les applications sous forme de jar peuvent être exécutées automatiquement.

Une archive jar contient un fichier manifest qui permet de préciser le contenu du jar et de fournir des informations sur celui-ci (classe principale, type de composants, signature ...).


### Commentaires

    /**class MainApp {

    }
    * ou
    class MainApp 
    {

    }
    */


    //Commentaires:
    //Pour un commentaire sur une seule ligne

    /*En bloc,
    *djzhfijfh
    */

    /** commentaires de documentation*/


### Objet et classe

En JS, l'on a vu les constructeurs.
En Java, on utilisera les objets, méthodes, classes ...
**Java est un langage orienté objet, chacun de nos fichiers représentera une classe.**
**Les conventions veulent que les classes, objets commencent par une majuscule.**

Une classe est quelque chose qui a un **nom** et des **attributs**.

 Exemples:
    siège -> nom
    assise, dossier,... -> attributs

    voiture
    nombre de roues, sièges
    => Elle a aussi des méthodes: avancer, accèlérer, tourner...
    Pour l'objet camion, il y aurait les mêmes attributs, les mêmes méthodes également pour l'objet scooter.
    Ce sont des véhicules = nom commun.

Ils **sont classés dans la catégorie véhicule**.
Ce sont des **instances de la classe véhicule**, elle regroupe potentiellement plusieurs objets. Elle va faire hériter des choses constantes aux objets.
Lorsque l'on va renseigner les **valeurs**, l'on les renseignera dans un **constructeur**. A chaque instance, on renseigne les nouvelles valeurs.
On est pas obligé de tout utiliser, et l'on peut en rajouter.

Exemple:
    Un avion hérite de la classe véhicule.

C'est le principe de base de la POO : **une classe est un objet**.   

**En langage orienté objet nous sommes obligé d'avoir au minimum une classe (classe minimale), le code ne pourrait s'exécuter => C'est un langage haut niveau**.

Pour créer un nouvel objet, on écrira que camion = **new** vehicule.
Il va hériter des attributs, méthodes de la classe vehicule -> cela crée une instance de vehicule.
New se rapporte au consctructeur.

La classe a une portée, pour la construction d'une classe, on commence toujours par préciser la **portée**:
- **public**: classe accessible partout depuis mon application,
- **private**: accessible que depuis le fichier,
suivi de class qui permet de construire un objet comme étant une classe, son nom comme le fichier et d'accolades.

=>**Obligation nom de fichier et nom de classe**.
=>**Une classe a toujours une fonction constructeur**.

Voir chat.java, chien.java et App.java:
Chaque fois que l'on fait un nouveau Chat => **instance de la classe**.

Le mot clef **this** fait référence au contexte.

Exemple (fichier App.java du dossier TestJava):

Construction d'une classe:
création fichier .java, le nom sera donné à la classe. 
Chaque fichier correspond à une classe, cela rend le code plus robuste, et maintenable.
Précision de la portée (public, private,...),
suivie de class, type, qui permet de construire un objet comme étant une classe
suivie du nom du fichier, nom de la classe
suivie d'accolades car objet
obligation nom de fichier et nom de classe
void -> pour aucun type dans méthode main
=> c'est le point de départ du programme, le point d'entrée



#### Constructeur 

    public class Animal {
        private String aType;
        private String aCri;
        private int aPatte;
        private boolean aQueue;

        public Animal(String type, String cri, int patte, boolean queue){
            this.aType = type;
            this.aCri = cri;
            this.aPatte = patte;
            this.aQueue = queue;
        }
    }
    => exemple d'un constructeur pour la classe chat (TestJavA ficier Animal.java);
    L' on déclare les variables qui correspondent aux  attributs de la classse.

Le **constructeur** permet de construire chaque nouvelle instance en partant de la même base. 
Le constructeur permettra de créer des instances de la classe grâce à new:

Exemple:
<<<<<<< HEAD
Dans une méthode, l'arguement doit être typé", lorsque c'est une classe on crée notre propre type.

Variable => minuscule
Classe qui sont des objets => majuscule


=======
>>>>>>> e1df4fcd1d6244df97220c50c01fb3f6f823eba4

Création d'instances de la classe Chat:

    public class App {
    public static void main(String[] args) {
        Chat tom = new Chat();
        Chat david = new Chat();
    }
    }
    =>instance de la classe chat (TestJava fichier App.java et Chat.java)

Son constructeur dans la classe Chat:

    public class Chat {
        public  Chat() {
            System.out.println("Le chat fait miaou-miaou" + " "+ this);
        }
    }
    =>Exécution App.java : Le chat fait miaou-miaou Chat@372f7a8d => identifiant de l'instance de Chat. Le nom et id de l'instance sont uniques.
    Chaque instance de chat aura un emplacement dans la mémoire qui lui est dédié, d'où l'id. Ces espaces sont différents, donc chacun peut faire une action différente de l'autre en même temps.

**Les arguments**:
En java tout est **typé**.
 public class Chat {
    public  Chat() {
        System.out.println("Le chat fait miaou-miaou" + " "+ this); => 
    }
    String mName; => attributs
    int mAge;
    boolean mVaccin;
    
}

#### Encapsulation

voir chat et app.

Permet de définir si on accès ou non depuis l'extérieur aux attributs.
=> private, pubic => encapsulation.

**On parle d'accesseurs, ou getter. Un accesseur est une méthode permettant de récupérer le contenu d'une donnée membre protégée**.
Rend accessible les données de notre classe même si pas en public.


On peut encapsuler également les données.

>Les méthodes comme System.out.println() s'exécute directement, ..., on peut importer des bibliothèques Java comme Scanner.
Mutateur inverse d'un accesseur.
Pour envoyer une valeur sans changer l'instance ->setter


Les méthodes comme System.out.println() s'exécute directement, ..., on peut importer des bibliothèques Java comme Scanner.

[getter setter](https://www.w3schools.com/java/java_encapsulation.asp)

### Héritage

Voir dossir TestJava fichier Animal.java et Chèvre.java:

    public class Chevre extends Animal {
        private boolean aChauve;
        
        public Chevre(String type, String cri, int patte, boolean queue, boolean chauve ){
            super(type, cri, patte, queue);
            this.aChauve = chauve;
        }
    }
    =>The extends keyword extends a class (indicates that a class is inherited from another class).In Java, it is possible to inherit attributes and methods from one class to another. We group the "inheritance concept" into two categories:subclass (child) - the class that inherits from another classsuperclass (parent) - the class being inherited fromTo inherit from a class, use the extends keyword.
    =>The super keyword refers to superclass (parent) objects.It is used to call superclass methods, and to access the superclass constructor.The most common use of the super keyword is to eliminate the confusion between superclasses and subclasses that have methods with the same name.

### Types

#### Les types primitifs

Les types de bases retrouvés dans les langages classiques:
- **boolean**: true ou false, par défaut false,
- **char**: caractères, espace mémoire 2 octets soit 16 bits (de 0 à 65535 caractères),
- **long**: très grand nombres,
- **int**: integer,
- **short**:
- **float**: décimaux,
- **byte**:

**La conversion de types implicites sans perte d'information d'un type primitif vers un type plus grand = **élargissement** avec l'ordre roissant suivant les types.

La maîtrise des types permet d'avoir des applications très performantes,  meilleure gestion de l'espace mémoire.

![les types primitifs en Java](img/../../TestJava/img/Les-types-primitifs-en-Java.jpg)

float et double:

[flota double](https://www.sololearn.com/Discuss/749938/*in-java-float-a-1-1f-what-is-this-f-stands-for)
>Attribuez une valeur à la variable. Lorsque v
affectez un nombre à virgule flottante à un `floa
ajoutez un `f` ou `F` au nombre pour indiquer
compilateur qu'il s'agit d'une valeur à virg
flottante simple précision.*/


*Type void et type any: void = aucun type et any = tous les types*.

### Constante

**final** mot clef qu'en POO, variable qui ne peut être changée.
final type nom en majuscule

### Bases numériques

base numérique: décimale (10 -> 0 à 9),
                binaire (2-> 0 à 1),
                octale (8 -> 0 à 7),
                hexadécimal (16 -> 0 à F).
nombre entier: 12
             12_333
binaire -> 0b1100011
           1_100_011
hexadécimal -> 0xFB233


## Open Classroom:

### Variables

>Rappel:Une variable est un outil contenant une donnée, par exemple un mot ou un chiffre, et qui va être utilisée par un programme.Un programme manipule constamment des variables, soit que l'on a définies, soit qu'il a créées.Les variables contiennent des **valeurs**, ces variables sont gérées et enregistrées par l'ordinateur. Pour savoir ce qu'elles contiennent nous leurs donons un nom.

#### Les nommer

Son nom doit reflèter son contenu.

Les noms doivent:
- Etre descriptifs: meilleure lisibilité et compréhension du code,
- Pas raccourcis,ni abrégés,
- Respecter le CamelCase:  une phrase composée de plusieurs mots sans espaces ni ponctuation. Le premier mot est écrit en minuscules et tous les autres mots commencent par une majuscule,

### Les déclarer

Pour utiliser les variables, il faut les créer, ou **déclarer**.
>Il existe plusieurs types de variables, en fonction du type de valeur qu'elles contiennent.

En Java, par exemple, si la variable contient un nombre entier elle sera déclarée en utilisant le mot clé **int** suivi du nom de la variable? On dit que ce sont des **int**.

Exemple:

    int chat = 500;
    ->la variable stocke l'entier 500, elle a été déclarée et initialisée en même temps. (Assignation d'une valeur de départ)

En Java, chaque instruction se termine par un **;**

Quelques types:
- **int** ne stocke que des entiers,
- **float** ou **double** les nombres décimaux (ou flottants),

#### Modifier les valeurs des variables avec les opérateurs

Une variable peut varier c'est à dire changer de valeur.
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

##### Ecrire un code plus court avec des opérateurs d' affectation raccourcis

Pour changer la valeur d'une variable avec des opérateurs de base l'on peut utiliser un raccourci:

    epargne = epargne + 100;
    =>
    epargne += 100;

Cela fonctionne donc avec:
-=
*=
/=

#### Manipuler d' autres données que les nombres

Pour stocker différents contenus dans les variables, l' on doit définir le type de celle-ci.
En effet, en fonction du type, les variables stockées dans la mémoire de l'ordinateur ne prennent pas la même place.

Il existe les variables:
- texte: **String**,
- entier: **int**,
- float: **double** ou **float**.
  
Exemple de déclaration de variables:

    String text = "blabla";
    int numberOfCat = 10;
    double percentage = 0.0d;

#### Les variables qui ne "changent pas"

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

#### Spécifier le bon type de variable

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

#### Les types numériques

Les types numériques sont:
- Les nombres entiers,
- Les nombres décimaux.
  
##### Les nombres entiers

Ils sont déclarés comme toutes autres variables, avec un type, nom et une valeur.

    int count = 10;
    ->variable de nom count, type int et valeur 10.

##### Les nombres décimaux

En Java,pour les décimaux il existe deux types différents:
- **double**,
- **float**.

**Ces deux types ont le même but. La différence est que double est deux fois plus précis que float, il propose plus de décimales après la virgule (float deux décimales après la virgule).**

    float lenght = 1876.19f;
    double width = 1258.6549745d;

    float lenght = 1256f.16566;
    =>lenght = 1256.16;

Il faut penser mémoire et décimale. De façon générale, en Java, l'on utilise le double par anticipation.

#### Mélanger des types numériques

Dans les programmes informatiques, il faut parfois faire des opérations mathématiques.
Cependant, les variables utilisées ne seront pas forcèment du même type (tant qu' elles restent numériques).
Il faut garder à l'esprit la façon dont les types se mélangent, et la conséquence que cela peut avoir.

Exemple:

    int a = 5;
    int b = 2;
    int c = a / b;
    =>c =2

    int a = 5;
    int b = 2;
    float c = a / b;
    =>c = 2.0;

    int a = 5;
    float b = 2;
    float c = a / b;
    =>c = 2.5;
    ou avec un cast

    int a = 5;
    int b = 2;
    float c = (float) a / b ;
    =>c = 2.5;

#### Les booléens

Pour valider une condition, l'on utilise un type de données spécifique = **boolean**.
Une variable de type boolean ne peut contenir que deux valeurs: **true** ou **false**.
Ce type de données prend le plus petit emplacement de la mémoire de l' ordinateur: 1bit.

Exemple:

        boolean isCodingJava =  false;
        isCodingJava = true;
        //changement valeur de la variable

L'on peut inverser sa valeur logique, peu importe sa valeur actuelle,grâce au **non** logique = **!**.

Exemple:

    boolean isCodingJava = true;
    isCodingJava = !isCodingJava;
    =>devient false

#### Le type String

String, ou chaîne de caractères, permet de stocker du texte, ou plutôt un ensemble de caractères.
Le String est un **objet**.

Exemple:

    String city = "Nice";
    String pet;
    String cat = "";

##### Concaténation des variables de type String

Exemple:

    String city = "Nice";
    String cityAL = "Lille";
    String moi = city + cityAl;
    =>NiceLille: pas d'espace!

    String city = "Nice";
    String cityAL = "Lille";
    String moi = city+ " " +cityAl;
    =>Nice Lille

L'on peut concaténer avec d'autres type de données:

    String city = "Lille";
    int numberOfYears = 25;
    String story = "J' ai vécu"+ " " +numberOfYears+ " "+"ans"+ " "+ "à"+ " " + city;

L'opérateur + permet la concaténation des chaînes et des nombres.

### Ecrire une fonction

#### Notion de classe

Une **classe** est un ensemble de:
- Variables, nommées **attributs**,
- Et de **comportements**, nommés **méthodes**.

Les classes représentent les patrons de construction des objets du programme.

Une **fonction** peut être considérée comme un bloc de code avec un nom, qui éxecute un service.
La fonction **main**: le service effectué est le programme lui-même.
Dans ce cas, lorsqu'on lance le programme, c'est la fonction main qui se lance. Elle est également appelée **point d'entrée**.

Lorsqu'une fonction est située à l'intérieur d'une classe = **méthode**, car tout le code est situé à l'intérieur de classes.

>Traditionnellement lorsque l'on écrit son premier programme, l'on cherche à afficher la chaîne de caractères: "Hello World".

    package hello;

    public class HelloWorld {
        //*Le programme commence ici*/
        public static void main(String[] args){
            System.out.printIn("Hello Wordl!");
        }
    }
    
    -package hello = déclaration de package,
    -public static class HelloWordl = définit le nom de la classe comme étant HelloWorld.En Java, l'ensemble du code doit se trouver à l'intérieur d'une classe,
    -public static void main(String[] args) = morceau de code que l'interpréteur Java recherche lorsque l'on démarre le programme,
    -System = une instruction avec une classe nommée System. Cette classe n'a pas besoin d'être instanciée pour être utilisée,
    - System.out.printIn("Hello Wordl!") = instruction qui affiche le message attendu.


>Deux étapes sont importantes pour qu'un programme Java se lance: la **compilation** et l'**interprétation**. Le compilateur intervient en amont pour prendre le code du développeur et le transformer en byteCode (ou code binaire-langage machine). Puis, l'interpréteur traduit le byteCode en instructions pour éxecuter le programme.

/** */ = commentaires de documentation

=>Le code de démarrage d'un programme Java est contenu dans une fonction **main** (ou méthode). Cette fontion est elle-
même contenue dans une classe, et cette classe appartient à un package.

#### Exécution du programme via le terminal

En Java, il y a une correspondance directe entre:
- les packages et les dossiers,
- les classes et les fichiers.

Pour éxécuter le programme sur l'ordinateur, l'on doit créer des dossiers qui correspondent aux packages, et des fichiers qui correspondent aux classes.
 
Etapes principales:
- Création dossier dans lequel sera tout le code. Cela correspond au dossier **root**,
- Dans ce dossier, l'on crée un dossier hello qui correspond au nom du package,
- Puis, création d'un fichier HelloWorld.java dans le dossier hello, cela correspond au nom de ma classe.

(Dans le programme HelloWorld: le code est écrit dans la méthode principale d' une classe HelloWorld. Méthode qui se trouve dans un package hello)


Une fois le code à l'intérieur du fichier, l'on doit le convertir en code éxecutable par une machine (code machine).
Quelque soit le langage de programmation, le code doit être traduit en un ensemble d'instructions qu'un ordinateur peut éxecuter = **code machine**.
Code difficile à écrire pour un humain.

Le langage dans lequel le code Java doit être transformé = **Bytecode**, il faut pour cela utiliser le **compilateur javac**.
C'est pour cela que les dossiers sont utiles.

Via le terminal: 
    dans le dossier root éxecuter

    $ javac hello/HelloWorld.java


## Exercices

### Syntaxe

[exercices de syntaxe](https://www.w3schools.com/java/java_syntax.asp)


    int x = 5, y = 6, z = 50;
    System.out.println(x + y + z);

    int myNum = 9;
    float myFloatNum = 8.99f;
    char myLetter = 'A';
    boolean myBool = false;
    String myText = "Hello World";

    double myDouble = 9.78d;
    int myInt = (int) myDouble;
    ->Le cast est le fait de forcer le compilateur à considérer une variable comme étant d’un type qui n’est pas le type déclaré ou le type réel de la variable.
    [cast Java](http://www.javacoding.fr/le-cast-en-java-downcasting-et-upcasting/)

    String txt = "Hello";
    System.out.println(txt.length());
    ->Use the correct method to print the length of the txt string

    String firstName = "John ";
    String lastName = "Doe";
    System.out.println(firstName.concat(lastName));
    ->Use the correct method to concatenate two strings

    String txt = "Hello Everybody";
    System.out.println(txt.indexOf("e"));
    ->Return the index (position) of the first occurrence of "e" in the following string

    int x = 5;
    int y = 10;
    Math.max(x, y);
    -> Use the correct method to find the highest value of x and y

    int time = 20;
    String result = (time < 18) ? "Good day." : "Good evening.";
    System.out.println(result); 
    ->Insert the missing parts to complete the following "short hand if...else statement" (ternary operator)

    int i = 1;
    while (i < 6) {
    System.out.println(i);
    i++;
    }
    ->Imprimer i tant que iest inférieur à 6

    String[] cars  = {"Volvo", "BMW", "Ford"};
    ->Create an array of type String called cars

    String[] cars = {"Volvo", "BMW", "Ford"};
    System.out.println(cars[1]);
    ->Print the second item in the cars array

    String[] cars = {"Volvo", "BMW", "Ford"};
    for (String i : cars ) {
    System.out.println(i);
    }
    ->Loop through the items in the cars array

    int[][] myNumbers = { {1, 2, 3, 4}, {5, 6, 7} };
    ->Insert the missing parts to create a two-dimensional array

    // Create a checkAge() method with an integer variable called age
    static void checkAge (int age) {
    // If age is less than 18, print "Access denied"
    if (age < 18) {
        System.out.println("Access denied"); 

    // If age is greater than, or equal to, 18, print "Access granted"
    } 
    else
    {
        System.out.println("Access granted"); 
    }

    } 

    public static void main(String[] args) { 
    // Call the checkAge method and pass along an age of 20
    
    checkAge
    (
    20
    );
    }


### Dossier TestJava

Dans cet exercice, Main correspond à la classe.

Ouvrir bloc-notes, puis le renommer MainApp.java.
Ouverture via VS Code.
**Notre fichier représente une classe**.
Il existe deux conventions avec les {}:

    class MainApp {
        
    }
    ou:
    class MainApp 
    {

    }
Java va toujours exécuter le premier main.

#### Fichier APP.java

    import java.util.Scanner;
    // import bibliothèque interne de Java, utilisation de la méthode Scanner

    public class App 
    {
        public static void main(String[] args)
        {
            Chat c = new Chat("David", 55, true);
            Chat felix = new Chat("Felix", 44, false);
            // System.out.println(c.mAge);
            // Affichage de l'attribut âge de c :55
            // System.out.println(c.mName);
            // => error the fiel Cht.mName is not visible car en private = encapsulé!
            // name(c);
            //=> appel fonction name pour le chat c
            // user(c);
            // presentation(c);
            felix.setVaccin(true);
            //envoie données à l'objet felix
            System.out.println(felix.getVaccin());
        }

        public static void name(Chat chat)
        {
            // System.out.println(c.mAge);
            // System.out.println(c.mName);
            // public. erreur, n'affiche pas la donnée
            // String cName = c.getName();
            System.out.println("c.mName: "+ chat.getName());
            // https://codegym.cc/fr/groups/posts/getters-et-setters-en-java
            // https://www.w3schools.com/java/java_encapsulation.asp
        }

        public static void user(Chat chat)
        {
            Scanner saisieUser = new Scanner(System.in);
            System.out.println("Veuillez saisir m pour faire miauler le chat sinon y pour faire aboyer le chien");
            String i = saisieUser.nextLine();
            String miaule = "m";
            System.out.println((i.equals(miaule)) ? "Le chat "+ chat.getName() +" fait miaou-miaou"  : "Le chien fait ouaf_ouaf");
            // La equals()méthode compare deux chaînes et renvoie true si les chaînes sont égales et false sinon.
        }

    }
    // Le constructeur a une mission primordiale: être le patron, tous les arguments doivent être présent

    /*
    * public static void presentation(Chat chat) {
        String question = "Voulez vous que je miaule? (y/n)";
        boolean continuePresentation = true;
        do {
            System.out.println(question);
            Scanner saisieUtilisateur = new Scanner(System.in);
            String resp = saisieUtilisateur.next();

            if (resp.equals("y")) {
                System.out.println(chat.getName() + "miaou");
                continuePresentation = false;
                saisieUtilisateur.close();
            } else if (resp.equals("n")) {
                    System.out.println("bye");
                    continuePresentation = false;
                    saisieUtilisateur.close();
            } else {
                question = "Je n'ai pas compris, y ou n?;
                continuePresentation = true;
            }       
        }
        while(continuePresentation);
    }
    */

#### PowerShell

Recherche power -> windows powershell, saisir le chemin après le chemin courant :cd suivi de ->  Desktop\GIT\TestJava.
Cela change le chemin courant (cd permet de changer le répertoire).
Puis ls entrée pour avoir le dossier et son contenu.

Ensuite, saisie de javac ./MainApp.java pour compiler le code.
![compilation](img/1-compilation_PowerShell.PNG)
![compilation](img/2-MainApp.class.PNG)

Le code pourra être exécuté => java MainApp
![compilation](img/3-execution.PNG)


#### Fichier MainApp.java

En langage orienté objet nous sommes obligé d'avoir au minimum une classe (classe minimale). Le code ne pourrait s'exécuter.
Ici = class MainApp. 

    public class MainApp 
    {
        public static void main (String[] args)
            {
            /*Signature, publique: accessible partout, la JVM peut y *avoir accès. Recherchée par Java:les arguments ou *paramètres Liste de String
            *Ce qui est dans la méthode sont des arguments
            *Dans méthode main de type void, on peut placer des arguments. Mais Java doit reconnaître la signature.
            *static est accessible ici*/

                System.out.println("Hello You!!!");

            */équivalent de console.log, on doit indiquer la sortie
            *System est un objet auquel on applique la méthode println*/
            }
    }

    public class MainApp 
    {
        public static void main (String[] args)
        {
            int maVariable = 36;
            /*déclaration d'une variable entier
            *déclaration variable pas d'espace, accent, espace. *Commence par une lettre ou underscore: camelCase ou *snake_case*/
            System.out.println(maVariable);
            maVariable = 37;
            System.out.println(maVariable);
            maVariable = maVariable + 1;
            System.out.println(maVariable);
            autreMethode();
            // ne fonctionne pas car dans la methode autreMethode pas de static, il faut permettre l'accès au code
        }
        //public void autreMethode()
        public static void autreMethode()
        {
            System.out.println("test");
            // rien ne s'affiche car pas invoqué dans main, il faut l'invoquer dans la méthode main
        }
    }
    // "index" appelé, exécuté, la méthode main sera exécutée, c'est l'index de l'index

    public class MainApp 
    {
        public static void main (String[] args)
        {
            final int MAVARIABLE = 36;
            System.out.println(MAVARIABLE); 
            /*MAVARIABLE = 37;
            *System.out.println(MAVARIABLE);
            *error because const*/
        }
    }

    public class MainApp 
    {
        public static void main (String[] args)
        {
            // final float PI = 3.14;
            // error
            // final double PI = 3.14;
            final float PI = 3.14f;
            System.out.println(PI);
            /*https://www.sololearn.com/Discuss/749938/*in-java-float-a-1-1f-what-is-this-f-stands-for
            *Attribuez une valeur à la variable. Lorsque vous *affectez un nombre à virgule flottante à un `float`, *ajoutez un `f` ou `F` au nombre pour indiquer au *compilateur qu'il s'agit d'une valeur à virgule *flottante simple précision.*/
        }
    }

##### Conditions

    public class MainApp 
    {
        public static void main (String[] args)
        {
            boolean value = (24 == 24);
            System.out.println(value);
            //renvoie true

            boolean value1 = (24 === 24);
            System.out.println(value);
            // renvoie true
            //comparaison d'expression

            int age = 24;
            int age1 = 20;
            boolean value = (age == age1);
            System.out.println(value);
            // envoie false

            int age2 = 24;
            int age3 = 24;
            boolean value1 = (age2 === age3);
            System.out.println(value1);
            // renvoie true
            int value4 = 24;
            if (value4 == 24){
                System.out.println(value4);
            }
            // renvoie 24
            if (value4 == 24){
                System.out.println(value4);
            }
            // ne renvoie rien

            int ageAd = 20;
            if (ageAd >= 18 && ageAd < 64){
                System.out.println(ageAd);
            }else{
                System.out.println("non");
            }
            ou
            if (ageAd >= 18 && ageAd < 64)
                System.out.println(ageAd);
            else
                System.out.println("non");
            ou
            String result = (ageAd >= 18 && ageAd < 64) ? "ageAd" : "non"; 
            System.out.println(result);

            //S'il est majeur, on vérifie qu'il a la majorité internationale
            if (ageAd >= 18 && ageAd < 64){
                System.out.println("Vous êtes majeur");
                if(ageAd >= 21){
                    System.out.println("Vous êtes majeur dans tous les pays");   
                }else{
                    System.out.println(" en France seulement");
                }
            }else{
                System.out.println("mineur");
            }

            switch (ageAd){
                case 17:
                    System.out.println("mineur");
                    break;
                case 18, 19, 20:
                    System.out.println("majeur en France");
                    break;
                default:
                    System.out.println("majeur dans tous les pays");
                    break;
            }
        }
    }

##### Boucles

    public class MainApp 
    {
        public static void main (String[] args)
        {
            int i = 0;
            while(i != 20){
                System.out.println(i);
                // i != 2 => boucle infinie, aucune condition d'arrêt: ajout d'incrémentation ou valeur pour en sortir
                // i+=2;
                // si l'on met un break à la place de i+=2 => une seule exécution
                if (i == 10){
                    break;
                }
                i++;
                // si i différent de 20, je renvoie i et si i == 10 stop
            }
            int i = 0;
            while(i != 20){
                if (i == 10){
                    continue;
                    // continue instruction interrompt une itération (dans la boucle), si une condition spécifiée se produit, et continue avec l'itération suivante dans la boucle.
                }
                i++;
                System.out.println(i);
            }
        }
    }

    public class MainApp 
    {
        public static void main (String[] args)
        {
            int i = 0;
            do{
                i++;
                if (i == 10){
                    continue;
                }
                System.out.println(i);
            }
            while(i != 20);
        }
    }

    public class MainApp 
    {
        public static void main (String[] args)
        {
            int i = 0;
            do{
                i++;
                if (i % 2 != 0){
                    continue;
                }
                System.out.println(i);
            }
            while(i != 20);
        }
        // affiche les nombres pairs, continu bloque les impairs suite à la condition if
    }

    //afficher saisie user: scanner. Pour que Java puisse lire ce que vous tapez au clavier, vous allez devoir utiliser un objet de type Scanner. Cet objet peut prendre différents paramètres. !import -> toujours en haut du code

    import java.util.Scanner;
    public class MainApp 
    {
        public static void main (String[] args)
        {
            Scanner valeurDebut = new Scanner(System.in);
            // instance de scanner
            System.out.println("Veuillez saisir un entier :");
            int i = valeurDebut.nextInt();
            Scanner valeurFin = new Scanner(System.in);
            System.out.println("Veuillez saisir un entier :");
            int fin = valeurFin.nextInt();
            valeurDebut.close();
            valeurFin.close();
            // attention à la fermeture du scanner
            
            if (i > fin){
                System.out.println("la valeur de début doit être plus petite que celle de fin");
            }
            else{
                System.out.println("Vous avez choisi: " + i +" "+ fin + ",les valeurs paires entre ces chiffres sont:");
                do{
                    i++;
                    if (i % 2 != 0){
                        continue;
                    }
                    System.out.println(i);
                }
                while(i != fin);
            }
        }
    }
    /

    public class MainApp 
    {
        public static void main (String[] args)
        {
            
            for (int i = 0; i < 10; i++){
                System.out.println(i);
            }
            
            // L’itération sur une collection à l’aide de structures de boucles traditionnelles comme la boucle for exige de connaître le nombre exact d’éléments dans la collection et elle permet également d’introduire des erreurs. Ce qui n’est pas du tout souhaité, surtout lorsque l’on traite du Big Data, car en plus de traiter une masse importante de données, la moindre erreur peut être fatale.
        }
    }

### Dossier Java_variable_de_classe_heritage

Variable de classe Java et héritage

1- Création de la classe abonnement, et création de deux instances de la classe.

2- Création d'une classe voiture.

3- Faire valeurs par défaut, dans une classe mère et fille.
Faire classe animal, et classe chat et chien.



## Nota Bene

\n: retour à la ligne
\t: tabulation
\f: nouvelle page (file)
\r: retour chariot avec saut de ligne
\b: retour en arrière

## Sources

[open classroom](https://openclassrooms.com/fr/courses/6173501-apprenez-a-programmer-en-java/6313896-declarez-des-variables)
[jar](https://fr.wikipedia.org/wiki/JAR_(format_de_fichier))
[Java SE et EE](https://www.ibm.com/docs/fr/odm/8.9.1?topic=application-java-se-java-ee-applications)
[sololearn](https://www.sololearn.com/Discuss/749938/*in-java-float-a-1-1f-what-is-this-f-stands-for)
[développons en Java](https://www.jmdoudoux.fr/java/dej/chap-javadoc.htm)