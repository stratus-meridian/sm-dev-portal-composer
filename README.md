# Composer template for  Stratus Meridian Developer Portal

## Usage

First you need to [install composer](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx).

> Note: The instructions below refer to the [global composer installation](https://getcomposer.org/doc/00-intro.md#globally).
You might need to replace `composer` with `php composer.phar` (or similar)
for your setup.

After that you can create the project:

```
composer create-project stratus-meridian/drupal8-composer-project:9.x-dev YOUR_DIRECTORY_NAME --no-interaction
```
## Always use composer to download modules
With `composer require ...` you can download new dependencies / modules that you additionally need to your
installation.

```
cd /YOUR_DIRECTORY_NAME/
composer require drupal/devel
```
## For CI Jobs
Run `composer install` so that you can download all dependencies / modules that are required for the  installation.

```
cd /your-directory/
composer install
```

## For Local Setup
If you'd like to test this distribution in your local quickly you can use `quick-start`

```
cd /your-directory/
composer quick-start
```
