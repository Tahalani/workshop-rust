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
    Exercice 7 : Retour de fonction Result<Self::Value, M::Error> et Option (comme Maybe)

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
