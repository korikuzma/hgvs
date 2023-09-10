# Dev Containers

Instructions for working with hgvs using Dev Containers

## [Prerequisites](https://code.visualstudio.com/docs/devcontainers/tutorial#_prerequisites)

Prerequisites section is from VS Code Dev Containers Tutorial.

* [Install VS Code](https://code.visualstudio.com/download)

  You must be using VS Code to use the Dev Containers

* Install Docker

  Docker is needed to create and manage your containers

  * Docker Desktop

    Download and install [Docker Desktop](https://www.docker.com/products/docker-desktop/), or an [alternative Docker option](https://code.visualstudio.com/remote/advancedcontainers/docker-options), like Docker on a remote host or Docker compliant CLI.

  * Start Docker

    Run the Docker Desktop application to start Docker. You will know it's running if you look in the activity tray and see the Docker whale icon.

    Docker might take a few minutes to start. If the whale icon is animated, it is probably still in the process of starting. You can click on the icon to see the status.

  * Check Docker

    Once Docker is running, you can confirm that everything is working by opening a new terminal window and typing the command:

    ```shell
    docker --version
    ```

* [Install Dev Containers extension](vscode:extension/ms-vscode-remote.remote-containers)

  The Dev Containers extension lets you run Visual Studio Code inside a Docker container.

  [Marketplace Link](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) (if viewing from browser)

## SeqRepo REST and UTA Dependencies

[SeqRepo REST](https://github.com/biocommons/seqrepo-rest-service) and [UTA](https://github.com/biocommons/uta) will point to remote services, as specified by the `containerEnv`. These services are only meant to be used during the hackathon and getting started materials. If using these services for other uses (such as in a production pipeline), we ask that you spin up a separate instance. More information can be found in their respective READMEs.

## Creating the Dev Container

Open the VS Code Command Palette: Shift + Command + P (Mac) / Ctrl + Shift + P (Windows/Linux)

Type and select the following inside the Command Palette: `> Dev Containers: Rebuild and Reopen in Container`

The Dev Container will be created and install the dependencies needed.

You should see `Dev Container: biocommons @ desktop-linux` on the bottom left hand corner of VS Code.


## Running tests

To run tests:

```shell
make test
```
