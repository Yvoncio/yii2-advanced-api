<p align="center">

    <h1 align="center">Yii 2 Advanced Project Template with api</h1>
    <br>
</p>

Yii2 Advanced Application Template with RESTful API configured. Take a look at http://budiirawan.com/setup-restful-api-yii2/ for more detail explanation

## Install Composer Packages
You need [Composer](http://getcomposer.org) installed first.
```
composer self-update
```
```
composer install
```

## Run Yii Init
Open terminal and go to the project folder and run

Mac/Linux
```
php ./init
```

Windows
```
init
```
Choose **development** environment and finish the steps.

## Configure Database
create your database and configure it in **common/config/main-local.php**

## Run Database Migration
This command will create new country table and populate its data

```
./yii migrate
```

## Enable Mod Rewrite if you use Apache
Make sure you already enable this mod. Follow this [Tutorial](http://stackoverflow.com/questions/869092/how-to-enable-mod-rewrite-for-apache-2-2)

DIRECTORY STRUCTURE
-------------------

```
api
    config/              contains shared configurations
    modules/             contains modules versions
    runtime/             contains files generated during runtime
    web/ 				 contains the entry script and Web resources
common
    config/              contains shared configurations
    mail/                contains view files for e-mails
    models/              contains model classes used in both backend and frontend
    tests/               contains tests for common classes    
console
    config/              contains console configurations
    controllers/         contains console controllers (commands)
    migrations/          contains database migrations
    models/              contains console-specific model classes
    runtime/             contains files generated during runtime
backend
    assets/              contains application assets such as JavaScript and CSS
    config/              contains backend configurations
    controllers/         contains Web controller classes
    models/              contains backend-specific model classes
    runtime/             contains files generated during runtime
    tests/               contains tests for backend application    
    views/               contains view files for the Web application
    web/                 contains the entry script and Web resources
frontend
    assets/              contains application assets such as JavaScript and CSS
    config/              contains frontend configurations
    controllers/         contains Web controller classes
    models/              contains frontend-specific model classes
    runtime/             contains files generated during runtime
    tests/               contains tests for frontend application
    views/               contains view files for the Web application
    web/                 contains the entry script and Web resources
    widgets/             contains frontend widgets
vendor/                  contains dependent 3rd-party packages
environments/            contains environment-based overrides
```
