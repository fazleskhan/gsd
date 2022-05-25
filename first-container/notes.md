docker image build -t fazleskhan/gsd:first-ctr .
docker image ls
docker login
docker image push fazleskhan/gsd:first-ctr
docker image rm fazleskhan/gsd:first-ctr
docker image ls
docker container run -d --name web -p 8000:8080 fazleskhan/gsd:first-ctr
docker container ls
browse http://localhost:8000/
docker container stop web
docker container ls -a
docker container start web
docker container stop
docker container rm web
docker container ls -a
To launch docker in interactive mode ==> docker container run -it --name test alpine sh
To leave a container running in interactive mode == > ctrl-P-Q
docker container rm test -f