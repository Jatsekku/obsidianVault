https://docs.docker.com/reference/cli/docker/

## Most Frequently used/Useful commands

| <nobr> Command </nobr>                                      | Description                                                                   |
| ----------------------------------------------------------- | ----------------------------------------------------------------------------- |
| <nobr>`docker buildx build -t yourImageTag .`</nobr>        | Build docker image in current directory, name it yoourContainerTag            |
| <nobr>`docker system prune -a`</nobr>                       | Remove all unused images. Images used by running containers won't be removed. |
| <nobr>`docker images -a`</nobr>                             | List built images.                                                            |
| <nobr>`docker ps -a`</nobr>                                 | List all containers.                                                          |
| <nobr>`docker run -i -t yourImageTag`</nobr>                | Interactively run container based on image named yourContainerTag             |
| <nobr>`docker image history --no-trunc yourImageTag`</nobr> | List image's  layers. Do not truncate the output                              |

## Alternative tools - comparison 
(GPT generated)

| **Feature**              | **Docker Desktop**                    | **VSCode Docker Extension**         | **CLI**                                     |
| ------------------------ | ------------------------------------- | ----------------------------------- | ------------------------------------------- |
| **Platform**             | Standalone application                | Extension within VS Code            | Standalone tool available in terminal       |
| **Interface**            | GUI + CLI                             | GUI integrated into VS Code         | CLI-only                                    |
| **Resource Management**  | Yes, configurable in Desktop settings | No, relies on Docker's settings     | Limited, manual control via commands        |
| **Container Debugging**  | Limited                               | Advanced, integrated with VS Code   | Requires additional setup or external tools |
| **Docker CLI Included**  | Yes                                   | Requires pre-installed Docker CLI   | Itself                                      |
| **Ease of Use**          | Easier for new users via GUI          | Better for developers in VS Code    | Best for advanced users or scripting        |
| **Syntax Highlighting**  | No                                    | Yes, for Dockerfiles and Compose    | No                                          |
| **Registry Integration** | Basic GUI for managing registries     | Advanced, integrated into editor    | Requires manual registry commands           |
| **Remote Development**   | Limited                               | Yes, supports remote Docker hosts   | Yes, via SSH or Docker context              |
| **System Requirements**  | More resource-intensive               | Lightweight as it builds on CLI     | Lightweight                                 |
| **Automation Support**   | Minimal                               | Supports VS Code tasks              | Excellent for scripting and CI/CD           |
| **Installation**         | Requires separate installation        | Requires Docker CLI to be installed | Core Docker tool                            |
