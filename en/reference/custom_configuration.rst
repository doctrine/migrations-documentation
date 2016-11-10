.. index::
   single: Custom Configuration

Custom Configuration
====================

The AbstracCommand provide a set of method setMigrationConfiguration method which allow you to set your own.

This allows you to to build doctrine migration integration into your application or framework.


Have a look and you will see a new class at the above location that looks like
the following:

.. code-block:: php

    use Doctrine\DBAL\Migrations\Configuration\Configuration;

    $configuration = new Configuration();
    $configuration->setMigrationsTableName(...);
    $configuration->setMigrationsDirectory(...);
    $configuration->setMigrationsNamespace(...);
    $configuration->registerMigrationsFromDirectory(...);

    //My command that extends Doctrine\DBAL\Migrations\Tools\Console\Command\AbstractCommand
    $command->setMigrationConfiguration($configuration);
