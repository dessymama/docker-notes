1. What docker pull does. docker pull downloads image from Docker Hub if the image is not on the system.
2. What docker images does. doxker images list all downloaded images.
3. What docker run does. docker run creates and starts a container from an image
4. What docker ps does. docker ps shows the running container.
5. Difference between docker stop and docker rm. docker stop,stops the container while rm deletes the container
6. A simple workflow using all six commands.



1.docker pull nginx
Docker checks the computer.
If the image exists → it will use it.
If it doesn't exist → it will download it from Docker Hub.

2. docker images
REPOSITORY   TAG            IMAGE ID
nginx              latest            xxxxxxxx
ubuntu           latest            yyyyyyyy
Shows the downloaded image

3. docker run nginx
Docker checks for the nginx image.
Downloads it if needed.
Creates a container.
Starts the container.

4. docker ps
CONTAINER ID
IMAGE
STATUS
PORTS
NAMES

5. docker stop 
docker stop 123abc

6. docker rm
docker rm container_name
