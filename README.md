# Workshop-rust

Ce guide vise à vous fournir une introduction claire et précise à l'apprentissage du langage de programmation Rust. Il comprendra des instructions détaillées pour l'installation de Cargo, l'outil de gestion de packages et de construction de Rust, ainsi que cinq exercices progressifs pour vous aider à renforcer vos compétences en programmation Rust.
Table des matières

    Installation de Cargo
    Exercice 1 : Récupération des arguments!
    Exercice 2 : Addition
    Exercice 3 : Recherche d'un élément dans un tableau
    Exercice 4 : Manipulation de référence/variable
    Exercice 5 : Création d'une structure de données
    Exercice 6 : Tableau de pointeur sur fonction
    Exercice 7 : Le type Option
    Exercice 8 : Traitement des erreurs
    Exercice 9 : Séparation et longueur des mots dans une chaîne de caractères
    Exercice 10 : Programmation orientée objet

# Exercice 0

Installation de Cargo

Avant de commencer à apprendre Rust, vous devez installer Cargo, l'outil de gestion de packages et de construction officiel de Rust. Voici comment procéder :

    1: curl https://sh.rustup.rs -sSf | sh
    2: cargo init workshop-rust
    3: cd workshop-rust
    4: cargo build --release && cp target/release/workshop_rust .
    5: ./workshop-rust

Félicitation vous avez fait votre premier hello world! en rust. ^^

# Exercice 1 : Récupération des arguments!

Compétence: récupérer les arguments.

L'exercice " Récupération des arguments" est un incontournable pour tout débutant en programmation. Il sert d'introduction simple à un nouveau langage de programmation.
L'objectif de cet exercice est de récupérer les arguments dans le main pour ensuite les afficher.
Pour vous aider, voici le lien de la doc officiel de Rust:
https://doc.rust-lang.org/book/

exemple :

    ./workshop_rust "vive le rust!"
    vive le rust!

# Exercice 2 : Addition

Compétence: création de fonction simple

Pour cette exercice commencez par créer un fichier ex02.rs dans le dossier src.
L'objectif de cet exercice est de créer une fonction qui prend en paramètre 2 int et qui retourne le résultat obtenu après les avoir additionner.
Ensuite, appeler la fonction dans le main en lui donnant deux floats donnés en paramètre puis afficher le résultat.

exemple :

    ./workshop_rust -21 -21
    resultat: -42

# Exercice 3 : Recherche d'un élément dans un tableau

Compétence: Tableau.

Pour cette exercice commencez par créer un fichier ex03.rs dans le dossier src.
Une fois crée vous pouvez commencer à créer une fonction qui prends un vecteur de Int list et un Int nbr paramètre, celle-ci retournera l'index de nbr dans list.
Ensuite, appeler la fonction dans le main en lui donnant un vecteur de Int qui contient {1, 2, 3} et un Int qui sera par exemple 3 puis afficher le résultat.

exemple :

    ./workshop_rust 3
    index: 2

# Exercice 4 : Manipulation de référence/variable

Compétence: Variable mutable / réference.

Doc: https://doc.rust-lang.org/std/keyword.mut.html

Dans cette exercice nous allons voir comment changer une chaînes de caractères en rust sans la retourner.
D'abord commencez par créer un fichier ex04.rs dans le dossier src.
Une fois fait créer une fonction qui prends une vecteur de Int {1, 2, 3} en paramètre, celle-ci ne retourne rien.
Dans cette fonction modifier le vecteur pour que chaque variable sois égale à elle même +1.

exemple :

    ./workshop_rust
    vec: 2,3,4

# Exercise 5 : Création d'une structure de données

Compétence: Structure.

Dans cette exercice ont va voir comment créer une structure la remplir et l'afficher
Comme les exercices précedents créer un fichier ex05.rs dans le dossier src.
Vous pouvez maintenant créer une structure Person qui contient deux Int (Id, Age), créer ensuite une fonction qui la remplie et l'affiche.

exemple :

    ./workshop_rust 87484548454 42
    struct -> id: 87484548454 age: 42

# Exercice 6 : Tableau de pointeur sur fonction

Compétence: Pointeur sur fonction.

Doc: https://doc.rust-lang.org/std/collections/struct.HashMap.html

Créer un fichier ex06.rs
Dans celui-ci créer deux fonction, une qui s'appelle fct1 et qui affiche "Fonction 1" et l'autre s'appelle fct2 et qui affiche "Fonction 2".
Maintenant créer une 3ème fonction qui prends une string (fct1 ou fct2) en paramètre.
Dans celle-ci créer un tableau de pointeur sur fonction qui lancera la fct1 ou fct2 en fonction de la string en paramètre.

exemple :

    ./workshop_rust fct1
    Fonction 1

    ./workshop_rust fct2
    Fonction 2

# Exercice 7 : Le type Option

Dans cet exercice, vous allez pratiquer la manipulation de l'Option en Rust. L'Option est un type spécial en Rust qui permet de représenter la présence ou l'absence d'une valeur.
Vous devez écrire une fonction "find_lenght" qui prend en paramètre une chaîne de caractères (String) et retourne la longueur de cette chaîne de caractères. Si la chaîne de caractères est vide, la fonction doit retourner None. Sinon, elle doit retourner Some(n), où n est la longueur de la chaîne de caractères.

exemple :

    ./workshop_rust "Hello World!"
    Lenght = 12

    ./workshop_rust ""
    String is empty !

# Exercice 8 : Traitement des erreurs avec Result

Dans cet exercice, vous allez pratiquer le traitement des erreurs en utilisant le type Result en Rust. Le type Result est utilisé pour représenter une opération qui peut réussir et renvoyer une valeur ou échouer et renvoyer une erreur.
Vous devez écrire une fonction appelée "division" qui prend en paramètre deux nombres entiers et renvoie le résultat de leur division. Cependant, si le deuxième nombre est zéro, la fonction doit renvoyer une erreur de division par zéro.

exemple :

    ./workshop_rust 8 2
    4

    ./workshop_rust 8 0
    Erreur : Division by zéro

# Exercice 9 : Séparation et longueur des mots dans une chaîne de caractères

Dans cet exercice, vous allez pratiquer la séparation d'une chaîne de caractères en mots à l'aide d'un séparateur (Vous l'avez deja fait en C :D), puis mesurer la longueur de chaque mot. Vous allez donc écrire une fonction qui prend une chaîne de caractères, sépare les mots et renvoie la longueur de chaque mot dans un vecteur.

exemple :

    ./workshop_rust "J'aime le Rust !"
    Mot 1: 6 caractères
    Mot 2: 2 caractères
    Mot 3: 4 caractères
    Mot 4: 1 caractères

# Exercice 10 : Programmation orientée objet

Dans cet exercice, vous allez pratiquer les concepts de la programmation orientée objet. Vous allez créer une structure de données appelée Rectangle pour représenter un rectangle et définir des méthodes associées pour manipuler cette structure. Le rectangle est défini par sa longueur et sa largeur. Vous devez implémenter des méthodes pour calculer l'aire et le périmètre du rectangle.

# Félicitations à vous d'avoir terminé les 10 exercices ! Vous avez accompli un excellent travail en parcourant ces exercices qui couvraient différents aspects de la programmation en Rust, allant de l'installation de Cargo à la manipulation des chaînes de caractères, des vecteurs et des erreurs. Vous avez développé vos compétences en résolution de problèmes, en manipulation de données et en utilisation des fonctionnalités clés du langage Rust.
