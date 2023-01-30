FROM mysql:8

COPY  ./initdb.d /docker-entrypoint-initdb.d

RUN chmod -R 775 /docker-entrypoint-initdb.d

COPY  my.cnf /etc/mysql/conf.d/my.cnf

RUN chmod -R 775 /etc/mysql/conf.d/my.cnf

CMD ["mysqld"]