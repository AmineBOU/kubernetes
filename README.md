# Following steps

docker network create my-network
docker run -d --name mysql-container --network my-network datascientest/mysql-k8s:1.0.0
docker run -d --name fastapi-container --network my-network -p 8000:8000 fastapi:v1
