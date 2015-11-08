# Getting Started

## Initial Flare Installation

First globally require the Flare installation package:
```
    composer global require "laravelflare/install"
```

Now to install Flare in your current directory (on an existing Laravel Project):

```
    flare install
```

If you would prefer to install Flare on a new Laravel (5.1 LTS) Project:

``` 
    flare install clean
```

If you have decided to run a clean install, you will need to run the Laravel Migrations which will create the user table:

```
    php artisan migrate
```

## Include the Flare Service Provider and Resources

Ensure that `LaravelFlare\Flare\FlareServiceProvider::class` has been added to your Application Service Providers list (in config/app.php) automatically and if it has not add it after the RouteServiceProvider.

Publish assets and config with:

```
    php artisan vendor:publish
```

## Create your first account

To login to the Flare Admin you will need a user account. Currently the only Auth provider is the built in Auth which uses, by default, the User model. To create your first user you can use the `make:user` artisan command:

```
    php artisan make:user
```

You will be prompted for a name, an email address and a password - an account will then be created for you.

**One complete, you are ready to login to the Flare Admin at /admin!**

