docker image build -t fazleskhan/gsd:swarm-stack .

docker image push fazleskhan/gsd:swarm-stack

docker stack deploy -c docker-compose.yml counter

docker stack ls

docker stack services counter

docker stack ps counter

browser => http://localhost:5000

In docker-compose.yml change replica count to 5

docker stack deploy -c docker-compose.yml counter

docker stack ps counter

docker stack rm counter