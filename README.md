# Doctrine Migrations Documentation

## How to Setup

1. ```git clone git@github.com:doctrine/migrations-documentation.git```
2. ```git submodule add https://github.com/doctrine/doctrine-sphinx-theme.git en/_theme```
3. ```git submodule update```
4. ```./bin/install-dependencies.sh```

## How to Generate

1. ```./bin/generate-docs.sh```

It will generate the documentation into the build directory of the checkout.