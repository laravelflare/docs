# Upgrading

## Upgrading to 0.1.6 from >0.1.1
- Re-publish Flare assets with `php artisan vendor:publish`

## Upgrading to 0.1.1
- Backup the `public/vendor/flare` folder before deleting it.

- Run `php artisan vendor:publish`.

- Finally copy any custom/modified public assets from your `public/vendor/flare` backup into the appropriate location (which may have changed).