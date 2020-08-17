# Drupal Commerce Domain Example

## Getting Started

Included in the project root is a Lando configuration file (`.lando.yml`). The
only prerequisites are that you must have Lando and Docker installed.

Lando - **3.0.9**
Docker - **2.3.0.3**

From the root of the project, run:

```bash
$ lando start
```

### Composer

This site uses composer and will require the following command to download assets.

```bash
$ lando composer install
```

### Import DB

A copy of the Database is provided as a starting point.

Run the following to import the DB:

```bash
$ lando db-import database-file.sql.gz
```

### Import Config

This site does include config and new changes will be included via config only.
Meaning the included DB will not be updated.

to import the config run the following:

```bash
$ lando drush cim -y
```
