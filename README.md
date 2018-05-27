
# How I did it
 * following https://api-platform.com/docs/distribution
 * composer create-project symfony/skeleton bookshop-api
 * cd bookshop-api
 * composer req api
 * bin/console doctrine:database:create
 * bin/console doctrine:schema:create
 * php -S 127.0.0.1:8000 -t public
 * composer req server --dev
 * bin/console server:run
 * create //src/Entity/Book.php and //src/Entity/Review.php
 * php bin/console doctrine:schema:update --force