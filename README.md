<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About LaravelRBAC

1.Install Laravel Breeze
2.Make Model for Role

```php

php artisan make:model Role -m
```

-   This artisan command will create Both the Role named Model and roles table as a migration file

```php

   php artisan make:migration create_roles_table --create=roles


```

-   Above code says when we want to create separate command for migration file.

-   Create Model Permission

```php
php artisan make:model Permission -m
```

3. Add columns in permissions and roles migration file ( $table->string('name');
   $table->string('slug');)

4. Create a new Migration file

```php

php artisan make:migration create_users_permission_table --create=users_permissions


```

```

php artisan make:migration create_users_roles_table --create=users_roles
```
