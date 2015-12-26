## mariadb container
Just a very simple mariadb container with port 3306 exposed and /var/log/mariadb volume

## To build
``docker build -t <container_tag_name> .``

## To run
``docker run -it -d -p 3306:3306 --name=<container_name> <image_name>``

## Example
``docker build -t mariadb_image .``

``docker run -it -d 3306:3306 --name=mariadb_container mariadb_image``
