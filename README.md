# Drupal Backend for Gatsby

This is a Drupal setup to pass API to Gatsby frontend.

## Installation

Clone the repository and run the blow commands.

```bash
composer install
```

It will install all the required modules, then create a new database to setup Drupal site.
After installation go to settings.php file and add the $settings['config_sync_directory'] variable as below.

```bash
$settings['config_sync_directory'] = '../config';
```

Now go to terminal and import the configurations using drush command.

```bash
drush cim
```

At last clear the cache.

```bash
drush cr
```