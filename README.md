# SAE31_2023 : Évaluation de menu

## Description du Projet
Ce projet consiste à évaluer l'efficacité d'un menu d'application en simulant des tests utilisateur et en analysant les résultats pour optimiser la navigation. Réalisé en trinôme, les programmes en Java permettent de visualiser les menus à tester et de synthétiser les résultats des tests.

### Contexte
Dans une application proposant un grand nombre d'actions différentes, il est fréquent de construire un menu qui présente à l'utilisateur toutes les possibilités qui lui sont offertes sous une forme hiérarchique. Cela peut prendre la forme d'une barre de menu pour les actions toujours disponibles, ou d'un menu contextuel pour les actions associées à l'élément d'interface sélectionné. Chaque option dans un menu peut correspondre à une action ou à un sous-menu, ce qui permet d'organiser les actions et d'éviter de proposer des listes trop longues. Le défaut de cette technique est que l'utilisateur risque de ne pas trouver l'action qui l'intéresse car elle est cachée dans un sous-menu. Il est donc très important de rendre la répartition intuitive.

### Base du menu
Le menu de notre application se base sur l'onglet `Paramètres` du navigateur `Opera GX`.

## Protocoles de Test
Liste des références correspondant aux protocoles de test :
- `a7dbf3d6-872a-11ee-bd67-525400125400` : Trouver l'action qui permet d'activer les raccourcis souris.
- `a7dc0800-872a-11ee-bd67-525400125400` : Modifier les IPFS/IPNS.
- `a7dc1386-872a-11ee-bd67-525400125400` : Définir comme fond d'écran le fond d'écran personnalisé "Batman".
- `a7dc1f59-872a-11ee-bd67-525400125400` : Effacer l'historique de navigation.
- `a7dc2a91-872a-11ee-bd67-525400125400` : Lancer Discord.exe qui vient d'être téléchargé.
- `a7dc372a-872a-11ee-bd67-525400125400` : Activer la fonctionnalité qui rend transparent le lecteur vidéo lors d'une lecture en Picture-in-Picture..
- `a7dc434a-872a-11ee-bd67-525400125400` : Activer ou désactiver les sons du navigateur.
- `a7dc4e77-872a-11ee-bd67-525400125400` : Définir la musique de fond pour : "Confluence - Dominik Kalajdzic".
- `a7dc5b07-872a-11ee-bd67-525400125400` : Ajouter ChatGPT à la barre latérale.
- `a9f5af1c-8632-11ee-bd67-525400125400` : Ajouter un fond d'écran personnalisé.

## Commandes de Compilation et d'Exécution
- `make run-tests` : compile le projet et lance le programme de tests.
- `make run-stats` : compile le projet et lance le programme de statistiques.
- `make build` : compile le projet.
- `make clean` : supprime le dossier build qui contient les classes compilées.

### Création d'archives JAR
- `make jar-tests` : crée une archive .jar du programme de tests.
- `make jar-stats` : crée une archive .jar du programme de statistiques.

## Analyse des Statistiques
Exemple de lecture des camemberts du programme de statistiques :
- `Réussite - 1` : Cela représente la bonne action, qui sera toujours à 1.
- `Échec - 10` : 10 mauvaises actions ont été confondues avec la bonne.
- `7 tests de 8` : 8 sous-menus ont été déployés dans 7 tests différents.
- `3 tests de 15` : 15 sous-menus ont été déployés dans 3 tests différents.

## Organisation des Ressources
- [Bibliothèque](./lib) : Utilisé pour se connecter à une base de données MariaDB
- [Base de données](./sql) : Sert à récupérer et générer les données des protocoles.
- [Fichiers sources](./src/fr/iutfbleau/sae31_2023) : Tous les fichiers de code de notre projet.

## Évaluation du Projet
Nous avons obtenu la note de 13.50/20 lors de ce projet.

---

© Baptiste BLANCHON, Ayoub AMMARA & Samet DURAN  
- [Sujet disponible ici](http://www.iut-fbleau.fr/sitebp/sae3/31_2023/R9O9Y6NMKZMEE0M1.php).
