## DigitalOcean

#### Docker

    docker-machine create \
        --driver digitalocean \
        --digitalocean-region "lon1" \
        --digitalocean-size "512mb" \
        --digitalocean-image ubuntu-16-04-x64 \
        --digitalocean-private-networking \
        --digitalocean-ipv6 \
        --digitalocean-access-token $TOKEN \
        $NAME
    docker-machine ls
    docker-machine ssh $NAME "docker swarm init --advertise-addr $IP" # initialise as a manager
    docker-machine rm $NAME

    docker node ls
