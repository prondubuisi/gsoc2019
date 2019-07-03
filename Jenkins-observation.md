# Setup 

## Recommended  Psalm Version
-  Psalm Stable version for CiviCore is version 3.4.0

## Instructions
- Add psalm.xml to root folder in repo
- Remove `packages ` and `ext ` files/directories from files to be analysed in psalm.xml as the are git ignored in civicore 

-  Set Psalm version in composer.json to 3.4.0

## Jenkins console commands 

- composer update
    
  - This is required to bump dependencies up as Psalm works with newer dependency version than CiviCore and failure to do this leads to errors

- composer require --dev vimeo/psalm:3.4.0

- add a psalm.xml file manually or with `./vendor/bin/psalm --init`

- ./vendor/bin/psalm .

## Observations

- Errors are reduced by more than 50% by removing `ext` and `packages` folder

- Psalm sees returning error messages as failure, so final build is marked as failed
