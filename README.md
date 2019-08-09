# Laravel Eloquent 5.8 - User Roles and Permissions (ACL) using Spatie Tutorial

## Getting Started

[ROME](https://itsolutionstuff.com/post/laravel-56-user-roles-and-permissions-acl-using-spatie-tutorialexample.html) - Code 


### Installing

```
composer require spatie/laravel-permission
```

Now open config/app.php file and add service provider and aliase.

```
'providers' => [

	....

	Spatie\Permission\PermissionServiceProvider::class,

],
```

We can also custom changes on Spatie package, so if you also want to changes then you can fire bellow command and get config file in config/permission.php.

```
php artisan vendor:publish --provider="Spatie\Permission\PermissionServiceProvider" --tag="config"
```

```
php artisan migrate
```

## Create Table using Migrations

So, if you install fresh project then you have already users table migration but if you don't have products table, so can create manually and other table can create using Spatie package command, so run bellow command and check migration file also.

```
php artisan vendor:publish --provider="Spatie\Permission\PermissionServiceProvider" --tag="migrations"

php artisan make:migrate create_products_table
```
## Install collective/html

```
composer require "laravelcollective/html 5.5.*"
```

