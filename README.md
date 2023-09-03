-----------------------------------------------------------
Runing the project
-----------------------------------------------------------
cd api
docker build -t myapp41 . 

-------------------------------------------------------------
Create a container
-------------------------------------------------------------
docker run --name myapp14_c -p 4000:4000 myapp41

-------------------------------------------------------------
Useful Commands
-------------------------------------------------------------
docker images  -> show images
docker ps -> show running containers
docker ps -a -> show all containers
docker image rm imageName -> delete imageName (it should not be in use)
docker image rm imageName -f -> delete imageName (force delete)
docker container rm containerName  -> delete container 
docker container rm containerName1 containerName2 -> delete container 
docker system prune -a (delete all containers and all images and wolumes)


---------------------------------------------------------------
create image /container with version/tag
---------------------------------------------------------------
docker build -t myapp:v1
docker run --name myapp_c -p 4000:4000 myapp:v1