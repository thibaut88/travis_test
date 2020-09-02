# travis_test 
[![NPM version](https://badge.fury.io/js/travis_test.svg)](https://npmjs.org/package/travis_test) 
[![Build Status](https://travis-ci.org/thibaut88/travis_test.svg?branch=master)](https://travis-ci.org/thibaut88/travis_test)

## Name 

Démonstration de Travis.

## Description

> Travis-CI est une technologie permettant de synchroniser vos projets et d'exécuter des tests unitaires pour le déploiement de vos applications stockées sur Github.

##Pour démarrer avec Travis CI en utilisant GitHub

 1. Allez sur Travis-ci.com et inscrivez-vous avec GitHub .
 2. Acceptez l'autorisation de Travis CI. Vous serez redirigé vers GitHub.
 3. Cliquez sur votre photo de profil en haut à droite de votre tableau de bord Travis, cliquez sur Paramètres, puis sur le bouton vert Activer , et sélectionnez les référentiels que vous souhaitez utiliser avec Travis CI.

Ou vous cliquez sur le bouton Activer tous les dépôts à l'aide des applications GitHub sur la page de démarrage pour simplement activer tous vos dépôts

## Usage
Si vous êtes propriétaire d'un projet sur Github et que vous avez les autorisations propriétaires (fork) alors la suite vous ait destinée.
Tout d'abord il faut créer un fichier .travis.yml à la racine du projet pour indiquer à Travis-CI ce qu'il doit faire.
```sh
touch .travis .yml
```

Puis configurer le fichier comme vous le voulez. Exemple :
```sh
language: php
php:
	- 5.3
	- 5.4
	- 7.1
```

On doit maintenat ajouter le .travis.ymlfichier à git, commit et push pour déclencher une build Travis CI.
Travis exécute uniquement les builds sur les commits que vous envoyez après avoir ajouté un fichier .travis.yml.

Pour finir, on peut vérifier la page d'état de construction pour voir si votre construction réussit ou échoue selon l'état de retour de la commande de construction en visitant le site de [Travis CI](https://travis-ci.org/) et en sélectionnant votre référentiel.

##Plus que d'exécuter des tests
Travis CI ne sert pas uniquement à exécuter des tests, il y a beaucoup d'autres choses que vous pouvez faire avec votre code:

- déployer sur des pages GitHub
- exécuter des applications sur Heroku
- télécharger RubyGems
- envoyer des notifications

## License

MIT © [Thibaut Marchal](https://github.com/thibaut88)
