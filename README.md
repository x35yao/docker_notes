# Docker notes

## Conepts:
- Image: A template of a container.

- Container: A instance of an image.
## Commands:
`docker -ps`:  

Show running containers.

`docker -ps -a`:

Show present containers(including both running and stopped containers).

`docker stop container_ID`:

Stops a container with ID "container_ID".

`docker images`: 

Show available images.

`docker run Image_name`: 

Run a container of the image 'Image_name'. It will go donwload it from docker hub if it is the image is not on the host machine.

`docker stop $(docker ps -a -q)`:

Stops all containers.

`docker rm container_name`:

Remove a container.

`docker rmi image_name`:

Remove a image.

`docker pull image_name`:

Pull an image without running it.

`docker run --name docker_name image_name`:

Run an image_name instance with name docker_name.

`docker run -it --rm -v $PWD:/tmp -w /tmp tensorflow/tensorflow bash`:

Run a bash in the tensorflow docker with in the PWD.

`docker run --gpus all -it --rm -v $PWD:/tmp -w /tmp tensorflow/tensorflow:latest-gpu bash:
`
Run a bash in the tensorflow docker with in the PWD. With GPU
