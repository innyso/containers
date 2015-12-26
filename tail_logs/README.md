## tail logs container
A simple container to tail any logs from another container


## To build
``docker build -t <container_tag_name> .``


## To run
``docker run -it --rm --name=<app>_logs --volume-from <app_container_name> <container_tag_name> <app_container_volume>``

## Example
``docker build -t tail_logs .``

``docker run -it --rm --name=mariadb_logs --volume-from mariadb_container tail_logs ./var/log/mariadb/mariadb.log``

