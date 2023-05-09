# Workshop-rust

Ce guide vise à vous fournir une introduction claire et précise à l'apprentissage du langage de programmation Rust. Il comprendra des instructions détaillées pour l'installation de Cargo, l'outil de gestion de packages et de construction de Rust, ainsi que cinq exercices progressifs pour vous aider à renforcer vos compétences en programmation Rust.
Table des matières

    Installation de Cargo
    Exercice 1 : Hello, World!
    Exercice 2 : Calculatrice basique
    Exercice 3 : Recherche d'un élément dans un tableau
    Exercice 4 : Manipulation de chaînes de caractères
    Exercice 5 : Création d'une structure de données

# Exercice 0

Installation de Cargo

Avant de commencer à apprendre Rust, vous devez installer Cargo, l'outil de gestion de packages et de construction officiel de Rust. Voici comment procéder :

curl https://sh.rustup.rs -sSf | sh

cargo init workshop-rust

cd workshop-rust

cargo build --release && cp target/release/workshop_rust .

./workshop-rust

Une fois l'installation terminée, vous devriez pouvoir exécuter la commande cargo depuis votre terminal ou invite de commande.

# Exercice 1 : Hello World!

L'exercice "Hello World!" est un incontournable pour tout débutant en programmation. Il sert d'introduction simple à un nouveau langage de programmation.
Tout d'abord créer un fichier ex01.
L'objectif de cet exercice est de créer un main qui permet d'ecrire "Hello World!" en Rust.
Pour vous aider, voici le lien de la doc officiel de Rust:
https://doc.rust-lang.org/book/

# Exercice 2 : Addition

L'objectif de cet exercice est de créer une fonction qui prend en paramètre 2 float et de retourner le résultat obtenu après les avoir additionner.

# Exercice 3
