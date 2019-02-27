# Mysql-drupal
Mysql 5.6 Docker image with some optimisations for Drupal 8

# How use it
Is possible to use this image pulling it directly from the Docker hub and create a container:
```
docker run --name test \
    -p 8080:80 \
    -v ${PWD}/index.php:/var/www/html/docroot/index.php \
    -d burdastyletech/mysql-drupal:5.6.0
```

## Image tagging
The image is tagged here and in Docker hub follows the tagging of mysql: the first two numbers represent the Mysql version(i.e. 5.6), the last number (the one used usually for bugs) represent some changes (bugs, improvements...) to the image.

## Build a new image
If you prefer to build a new image just run:
```
docker image build -t {your/image/name}:{your/tag} .
```


