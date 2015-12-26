FROM fedora

RUN dnf -y update && \
dnf install -y mariadb mariadb-server && \
mysql_install_db && \
chown -R mysql:mysql /var/lib/mysql

VOLUME ["/var/log/mariadb"]

EXPOSE 3306
ENTRYPOINT ["/usr/bin/mysqld_safe"]
