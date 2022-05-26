docker compose version

docker compose up -d

docker image ls

docker container ls

browse => http://localhost:5000

docker compose down

docker swarm init

For HA deployments

  docker swarm init --advertise-addr=192.168.0.20

  docker swarm join-token manager

  docker swarm join-token worker

docker node ls

docker service create --name web -p 8080:8080 --replicas 3 fazleskhan/gsd:first-ctr

docker service ls

docker container ls

docker service ps web

browse => http://localhost:8080

docker service scale web=10

docker container ls