FROM mysql:5.7

# Create database & Application User
ENV MYSQL_DATABASE usersapidb
ENV MYSQL_USER apiuser
ENV MYSQL_PASSWORD p@ssw0rd

# All scripts in docker-entrypoint-initdb.d/ are automatically executed during container startup
COPY users.sql /docker-entrypoint-initdb.d/