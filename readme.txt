- composer init -n
    -> ne pose pas de questions, génère directement le fichier composer.json

- composer requiresymfony/var-dumper
    -> permet d'avoir accès à : dd()
        ex : dd($products); -> permet de voir ce que renvoie la variable $products
- au début du fichier :
    require 'vendor/autoload.php';

- je mets dans le fichier composer.json :
    "autoload": {
        "psr-4": {
            "App\\": "src/"
        }
    }

- composer dump-autoload
    -> met à jour l'autoloader

Tests unitaires:
- phpunit.de
- composer require --dev phpunit/phpunit "^8"
- créer dossier tests
- dans le terminal : ./vendor/bin/phpunit
    -> documentation
- dans le terminal : ./vendor/bin/phpunit tests
    -> résultats des tests
- plugin PHPUnit Test Explorer