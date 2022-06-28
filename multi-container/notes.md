docker compose version

  Install Docker Compose on Windows Server 2019
  https://docs.docker.com/compose/install/compose-plugin/#install-compose-on-windows-server
  [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12
  Invoke-WebRequest "https://github.com/docker/compose/releases/download/v2.6.1/docker-compose-Windows-x86_64.exe" -UseBasicParsing -OutFile $Env:ProgramFiles\Docker\docker-compose.exe
  The version of docker installed at this time is 20.10.9 and does not support docker plugins.
  On Windows Server 2019 substitute 'docker-compose' for 'docker compose'

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