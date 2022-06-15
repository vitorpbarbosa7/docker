Docker image delete:
docker images | awk 'FNR == 2 {print $3}' | xargs docker image rm

docker stop kedro_container && docker rm kedro_container

docker run -itd --name kedro_container kedro_docker

docker exec -it kedro_container bash
