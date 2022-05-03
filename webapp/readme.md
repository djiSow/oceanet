## Installation

````bash
composer install # installe les dépendances php
npm install # installe les dépendances javascript
npm run dev # Lance une build des assets en mode dev

php -S localhost:8080 -t public # lance un serveur php sur le port 8080 en local pointant sur le dossier public
```
````

Remarques:

- la configuration des identifiants de la base de données se fait dans le fichier .env
- lors du développement, il est préférable de lancer `npm run dev-server` afin de démarrer un serveur de build qui permet d'éviter de relancer la commande `npm run dev` lors de chaque modification des assets (.js, etc...)

## Commit rules

Tout les commits doivent être prefixés par (setup, add, feat, fix, remove, dump, etc...) et se terminer par une briève description des modifications apportées.

Exemple: `git commit -m "<action>(contexte): description"`

- fix(auth): faute d'orthographe sur la variable ...
- feat(register): enregistrement d'un utilisateur
