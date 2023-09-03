-----------------------------------------------------------
Runing the project
-----------------------------------------------------------
cd api  <br/>
docker build -t myapp41 . <br/>

-------------------------------------------------------------
Create a container
-------------------------------------------------------------
docker run --name myapp14_c -p 4000:4000 myapp41  <br/>

-------------------------------------------------------------
Useful Commands
-------------------------------------------------------------
docker images  -> show images  <br/>
docker ps -> show running containers  <br/>
docker ps -a -> show all containers  <br/>
docker image rm imageName -> delete imageName (it should not be in use)  <br/>
docker image rm imageName -f -> delete imageName (force delete)  <br/>
docker container rm containerName  -> delete container <br/>
docker container rm containerName1 containerName2 -> delete container <br/>
docker system prune -a (delete all containers and all images and wolumes)  <br/>


---------------------------------------------------------------
create image /container with version/tag
---------------------------------------------------------------
docker build -t myapp:v1  <br/>
docker run --name myapp_c -p 4000:4000 myapp:v1  <br/>
