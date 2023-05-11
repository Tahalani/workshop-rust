# Workshop-rust

Ce guide vise à vous fournir une introduction claire et précise à l'apprentissage du langage de programmation Rust. Il comprendra des instructions détaillées pour l'installation de Cargo, l'outil de gestion de packages et de construction de Rust, ainsi que cinq exercices progressifs pour vous aider à renforcer vos compétences en programmation Rust.
Table des matières

    Installation de Cargo
    Exercice 1 : Récupération des arguments!
    Exercice 2 : Addition
    Exercice 3 : Recherche d'un élément dans un tableau
    Exercice 4 : Manipulation de chaînes de caractères
    Exercice 5 : Création d'une structure de données

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

L'exercice " Récupération des arguments" est un incontournable pour tout débutant en programmation. Il sert d'introduction simple à un nouveau langage de programmation.
L'objectif de cet exercice est de récupérer les arguments dans le main pour ensuite les afficher.
Pour vous aider, voici le lien de la doc officiel de Rust:
https://doc.rust-lang.org/book/

exemple :

    ./workshop_rust "vive le rust!"
    vive le rust!

# Exercice 2 : Addition

Pour cette exercice commencez par créer un fichier ex02.rs dans le dossier src.
L'objectif de cet exercice est de créer une fonction qui prend en paramètre 2 int et qui retourne le résultat obtenu après les avoir additionner.
Ensuite, appeler la fonction dans le main en lui donnant deux floats donnés en paramètre puis afficher le résultat.

exemple :

    ./workshop_rust -21 -21
    resultat: -42

# Exercice 3 : Recherche d'un élément dans un tableau

Pour cette exercice commencez par créer un fichier ex03.rs dans le dossier src.
une fois crée vous pouvez commencer à créer une fonction qui prends un vec<Int> list et un int nbr paramètre,
celle ci retournera l'index de nbr dans list.
Ensuite, appeler la fonction dans le main en lui donnant un vec<Int> qui contient {1, 2, 3} et un int qui sera par exemple 3 puis afficher le résultat.

exemple :
    ./workshop_rust
    index: 2
    
