# proyecto-multimedial

## Create Database
* Database: pharmacy	
* Encoding: utf8_general_ci

## Install composer
Move to the project root folder and run from console
```composer install```

## Generate getters and setters
If you make some changes on the entities run ```php vendor/bin/doctrine orm:generate-entities .```

## Make changes on the Database
Run

```php vendor/bin/doctrine orm:schema-tool:update --force```

## Functions
All the utilities needed for the project backend interaction are placed at the **functions** folder.

```
.
+-- composer.json
|   .
|   .
|   .
+-- entities
|   +-- Agency.php
|   +-- Bill.php
+-- reports
|   +-- factura
|   +-- inventario
|   +-- proveedor
|   +-- user
+-- src
|   +-- functions
|   |   +-- bill_functions.php
|   |   +-- client_functions.php
|   |   +-- medicine_functions.php
|   |   +-- user_functions.php
|   +-- test_creations.php
|   +-- tests.php
|   .
|   .
|   .
```

## Reports

Inventario just call inventario.
Factura just call factura($id), id as bill(id)
Proveedor just call proveedor()
User just call user($id), id as client(id), show bills of a user.

