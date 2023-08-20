# Laravel Spatie

## Configuration
You can install the package via composer
```sh
 composer require spatie/laravel-permission
```

The service provider will automatically get registered. Or you may manually add the service provider in your config/app.php file:
```sh
'providers' => [
    // ...
    Spatie\Permission\PermissionServiceProvider::class,
];
```

You should publish the migration and the config/permission.php config file with:
```sh
php artisan vendor:publish --provider="Spatie\Permission\PermissionServiceProvider"
```

Clear your config cache. This package requires access to the permission config. Generally it's bad practice to do config-caching in a development environment. If you've been caching configurations locally, clear your config cache with either of these commands:
```sh
php artisan optimize:clear

#or

 php artisan config:clear
```

Run the migrations: After the config and migration have been published and configured, you can create the tables for this package by running:
```sh
php artisan migrate
```




## Reference
Laravel Spatie (https://spatie.be/)


## Author 
[Irfan Yasin](https://github.com/alirfanyasin)
