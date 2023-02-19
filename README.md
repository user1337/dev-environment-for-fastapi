0.
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)

docker stop fastapi-container
docker rm fastapi-container

docker ps

1.
docker build -t fastapi-image .

2.
docker images

3.
docker run --name fastapi-container -p 8080:80 fastapi-image
docker run --name fastapi-container -p 8080:80 -d fastapi-image

http://localhost:8080