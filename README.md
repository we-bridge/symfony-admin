
Symfony Admin Edition
========================

Welcome to the Symfony Admin Edition - a fully-functional Symfony2
application that you can use as the skeleton for your new applications
that requires a Admin backend.

This document contains information on how to download, install, and start
using Symfony. For a more detailed explanation, see the [Installation][1]
chapter of the Symfony Documentation.

1) Installing the Standard Edition
----------------------------------

When it comes to installing the Symfony Standard Edition, you have the
following options.

### Use Composer (*recommended*)

As Symfony uses [Composer][2] to manage its dependencies, the recommended way
to create a new project is to use it.

If you don't have Composer yet, download it following the instructions on
http://getcomposer.org/ or just run the following command:

    curl -s http://getcomposer.org/installer | php

Then, use the `create-project` command to generate a new Symfony application:

    php composer.phar create-project symfony/framework-standard-edition path/to/install

Composer will install Symfony and all its dependencies under the
`path/to/install` directory.

### Download an Archive File

To quickly test Symfony, you can also download an [archive][3] of the Standard
Edition and unpack it somewhere under your web server root directory.

If you downloaded an archive "without vendors", you also need to install all
the necessary dependencies. Download composer (see above) and run the
following command:

    php composer.phar install

2) Checking your System Configuration
-------------------------------------

Before starting coding, make sure that your local system is properly
configured for Symfony.

Execute the `check.php` script from the command line:

    php app/check.php

The script returns a status code of `0` if all mandatory requirements are met,
`1` otherwise.

Access the `config.php` script from a browser:

    http://localhost/path-to-project/web/config.php

If you get any warnings or recommendations, fix them before moving on.

What's inside?
---------------

The Symfony Standard Edition is configured with the following defaults:

  * Twig is the only configured template engine;

  * Doctrine ORM/DBAL is configured;

  * Swiftmailer is configured;

  * Annotations for everything are enabled.

  * Sonata Admin bundle is configured in /admin

  * FOSUserBundle is configured to manage your users

It comes pre-configured with the following bundles:

  * **FrameworkBundle** - The core Symfony framework bundle


  * [**SensioFrameworkExtraBundle**][6] - Adds several enhancements, including
    template and routing annotation capability

  * [**DoctrineBundle**][7] - Adds support for the Doctrine ORM

  * [**TwigBundle**][8] - Adds support for the Twig templating engine

  * [**SecurityBundle**][9] - Adds security by integrating Symfony's security
    component

  * [**SwiftmailerBundle**][10] - Adds support for Swiftmailer, a library for
    sending emails

  * [**MonologBundle**][11] - Adds support for Monolog, a logging library

  * [**AsseticBundle**][12] - Adds support for Assetic, an asset processing
    library

  * **WebProfilerBundle** (in dev/test env) - Adds profiling functionality and
    the web debug toolbar

  * **SensioDistributionBundle** (in dev/test env) - Adds functionality for
    configuring and working with Symfony distributions

  * [**SensioGeneratorBundle**][13] (in dev/test env) - Adds code generation
    capabilities

  * **SonataAdminBundle** - A bundle to generate admin interface

  * **FOSUSerBundle** - A bundle to manage users login/registration/forget password


All libraries and bundles included in the Symfony Standard Edition are
released under the MIT or BSD license.

Enjoy!

[1]:  http://symfony.com/doc/2.5/book/installation.html
[2]:  http://getcomposer.org/
[3]:  http://symfony.com/download
[4]:  http://symfony.com/doc/2.5/quick_tour/the_big_picture.html
[5]:  http://symfony.com/doc/2.5/index.html
[6]:  http://symfony.com/doc/2.5/bundles/SensioFrameworkExtraBundle/index.html
[7]:  http://symfony.com/doc/2.5/book/doctrine.html
[8]:  http://symfony.com/doc/2.5/book/templating.html
[9]:  http://symfony.com/doc/2.5/book/security.html
[10]: http://symfony.com/doc/2.5/cookbook/email.html
[11]: http://symfony.com/doc/2.5/cookbook/logging/monolog.html
[12]: http://symfony.com/doc/2.5/cookbook/assetic/asset_management.html
[13]: http://symfony.com/doc/2.5/bundles/SensioGeneratorBundle/index.html
