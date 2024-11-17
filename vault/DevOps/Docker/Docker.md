## Short intro 
- Build and run environments that are customized Linux instances
- Manage [[#image|images]] and [[#container|containers]]

## Architecture
- Docker Client - basically [[Docker CLI|CLI]] that handles REST API calls to docker host (UNIX sockets or network interface).
- Docker Compose is another client that allows managing set of [[#container|containers]].
- Docker Host - daemon that is responsible for communication with clients. 
  Handling all logic associated with building, running and managing [[#container|containers]] in general.
-  Docker Registries - servers that stores docker [[#image|images]]. [Docker Hub](https://hub.docker.com/) is an example of publicly accessible server that anyone can use. It's also possible to use own, self-hosted registry.
  ![[DockerArchitecture_overview.png]]
## Images vs Containers 

### Image 
- It's immutable, read-only template that tells docker daemon how to create container.
- Consist all needed files, libraries, binaries
- Made of layers (incremental changes in reference to previous state) defined by [[Dockerfile]].
- Usually based on other images accessible from registry.
- May be pushed into registry as a result of image build process

## Container 
- Runnable instance of an image.
- Changes in container are not persisted by default.
- Relatively isolated from host OS (sandboxes process)

## References
- https://docs.docker.com/get-started/docker-overview/#docker-registries
