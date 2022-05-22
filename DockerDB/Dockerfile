FROM mysql:5.7.38


ENV MYSQL_DATABASE=sample \
    MYSQL_ROOT_PASSWORD=samplepass \
    MYSQL_USER=sampleuser \
    MYSQL_PASSWORD=samplepass

ADD sql/db.sql /docker-entrypoint-initdb.d

EXPOSE 3306

# docker build -t mysqlodiaz -f .\DockerDB\Dockerfile
# docker run -d -p 6603:3306 --name testmysql mysqlodiaz