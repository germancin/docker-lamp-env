FROM mysql:5.7

RUN apt-get -qq update && \
    apt-get install  -y \
    tree \
    vim  && \
    mkdir -p /var/database/ && \
    chmod -R 777 /var/database/

#comment
WORKDIR /var/database/