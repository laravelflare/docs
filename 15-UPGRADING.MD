# Upgrading

## Upgrading to 0.1.15 from >0.1.1
- Remove Flare assets and config in the following locations:

`config/flare.php`
`resources/vendor/flare/`
`public/vendor/flare`

*Backup first if you've made changes from the defaults*

- Republish the assets and config:
`php artisan vendor:publish`

Reconfigure your config and reapply any changes made.



## Upgrading to 0.1.1
- Backup the `public/vendor/flare` folder before deleting it.

- Run `php artisan vendor:publish`.

- Finally copy any custom/modified public assets from your `public/vendor/flare` backup into the appropriate location (which may have changed).