# PRACTICA 1

## 1.1 - Haz una instalación limpia de Symfony

```bash
symfony new mpwar21-frameworks-<grupo> --version=~5.2
composer create-project symfony/skeleton mpwar21-frameworks-<grupo> ~5.2
```
## 1.2 - Añade un página en la ruta /hello que muestre el texto “Hello World”

Antes de crear el primer controlador, se debe de instalar lo siguiente:

```bash
$ composer require symfony/maker-bundle --dev
$ composer require doctrine/annotations
```
NOTA: Para evitar este error: Message: "There are no commands defined in the "make" namespace.

Creo mi primer controlador

```bash
$ symfony console make:controller HelloWorldController
```# docker-exercises
