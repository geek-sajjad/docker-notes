# Docker
docker is a container technology: A tool for creating and managing containers

## Container
  A standardized unit of software.
  A package of code and dependencies to run that code.
  tha same container always yields exact same application and execution behavior! no matter where or by whom is might be executed.

  Docker simplifies the creation and management of such containers.
  
  it should be easy to share a common development environment   / setup (new) employees and colleagues

## Commands
`docker build .`

`docker run -p 3000:3000 <image_hash>`

`docker ps -a`

`docker stop <name>`

`docker attach <container_hash>`

`docker logs <container_hash>`

`docker logs -f <container_hash>`

## images
images like blueprint for creating containers, you can build multiple containers from image contains code + required tools/runtime

### finding/creating images
* use and existing, pre-build image e.g: docker hub
  * `docker run node`
  * `docker run -it node`
  * `docker run -p <my_port>:<docker_container_port> <image_hash>`
* creating your own custom image (write your own Dockerfile based on another image)
## containers
  * `docker build ./`
the running unit of software, Multiple containers can be build created based on one image.
