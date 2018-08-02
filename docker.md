# Docker

## General
| Command                                                                        | Description                                          |
|--------------------------------------------------------------------------------|------------------------------------------------------|
| Ctrl + P + Q                                                                   | Exit box but keep it running                         |
| docker run -it --name <name>                                                   | Run a docker box with in interactive tty with a name |
| docker attach <name>                                                           | Attach the running docker box                        |
| docker ps                                                                      | List running boxes                                   |
| exit                                                                           | Close and shutdown box                               |
| docker images                                                                  | List docker images                                   |
| docker rmi <name>                                                              | Remove docker image                                  |
| docker build -t <container_name> .                                             | Build the docker box in the current directory        |
| docker run -it --rm --name <box_name> <container_name>                         | Run the docker build in box                          |
| docker run -it -p <local_port>:<container_port> --name <name> <container_name> | Run container with port mapping                      |
| docker start                                                                   | Start docker container detached                      |
| docker rm -f <name>                                                            | Remove container                                     |
|||

