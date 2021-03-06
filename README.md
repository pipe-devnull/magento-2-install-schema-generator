# Install Schema Generator

[![Latest Stable Version](https://img.shields.io/packagist/v/blackbird/installschemagenerator.svg?style=flat-square)](https://packagist.org/packages/blackbird/installschemagenerator)
[![License: MIT](https://img.shields.io/github/license/blackbird-agency/magento-2-install-schema-generator.svg?style=flat-square)](./LICENSE) 

**An extension for Magento 2 by Blackbird Agency**

## Synopsis

This project is a developer tool destined to speed up the tables creation's scripts of a Magento 2 module.
The purpose of this project is to make easier to create extra tables for your Magento 2 modules.
For example, you love the Phpmyadmin UI and have designed your tables with it. But now you have to write the entire 
setup script for your Magento 2 module... If only you were allowed to generate this setup script from your tables...
And here we are! That's why we offer you this module: it allows you to generate your InstallSchema.php setup file 
throught your database tables.

## How to use it

Requirements:

- You should have initialized a databasse and created your table(s)

You can generate the setup file via two methods:

- CLI command
- UI Backend

### CLI Command

Allowed CLI commands:

php magento isg:generate [tables...]

options:

-n : custom namespace name for the file
-l : location where to generate the file

### UI Backend

- Connect to your Magento 2 admin panel, then go to System => Install Schema Generator
- Insert your custom namespace
- Select the tables to generate into a InstallSchema.php setup file
- Download your file and enjoy it

![alt tag](https://black.bird.eu/media/wysiwyg/images/screen_backend_isg.jpg)

## Setup

### Get the package

**Zip Package:**

Unzip the package in app/code/Blackbird/InstallSchemaGenerator.

**Composer Package:**

```
composer require blackbird/installschemagenerator
```

### Install the module

Then, run the following magento command:

```
php bin/magento setup:upgrade
```

**If you are in production mode, do not forget to recompile and redeploy the static resources.**

## Support

Raise a [request](https://github.com/blackbird-agency/magento-2-install-schema-generator/issues).

## Authors

- **Thomas Klein** - *Initial work* - [It's me!](https://github.com/thomas-blackbird)
- **Blackbird Team** - *Contributor* - [They're awesome!](https://github.com/blackbird-agency)

## Contact

For further information, contact us:

- by email: hello@bird.eu
- or by form: [https://black.bird.eu/en/contacts/](https://black.bird.eu/contacts/)

## Licence

This project is licensed under the Blackbird Policy License - see the [LICENSE](./LICENSE) link for details.

***That's all folks!***
