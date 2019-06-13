# shiny-verse

Shiny server, based on the [Rocker shiny-verse](https://hub.docker.com/r/rocker/shiny-verse), for CyVerse VICE. 

[![Project Supported by CyVerse](https://img.shields.io/badge/Supported%20by-CyVerse-blue.svg)](https://www.cyverse.org) [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)

DockerHub        | description                               | size   | metrics | build status 
---------------- | ----------------------------------------- | ------ | ------- | --------------
[![DockerHub](https://img.shields.io/badge/DockerHub-brightgreen.svg?style=popout&logo=Docker)](https://hub.docker.com/r/cyversevice/shiny-verse) | Shiny Server | [![](https://images.microbadger.com/badges/image/cyversevice/shiny-verse.svg)](https://microbadger.com/images/cyversevice/shiny-verse) | [![](https://img.shields.io/docker/pulls/cyversevice/shiny-verse.svg)](https://hub.docker.com/r/cyversevice/shiny-verse)  |  [![](https://img.shields.io/docker/automated/cyversevice/shiny-verse.svg)](https://hub.docker.com/r/cyversevice/shiny-verse/builds)

VICE containers  | tag version                               | size   | metrics | build status 
---------------- | ----------------------------------------- | ------ | ------- | --------------
[![VICE](https://img.shields.io/badge/CyVerse-VICE-blue.svg?style=popout&logo=Docker&color=#1488C6)]()| latest | [![](https://images.microbadger.com/badges/image/cyversevice/shiny-verse.svg)](https://microbadger.com/images/cyversevice/shiny-verse) | [![](https://img.shields.io/docker/pulls/cyversevice/shiny-verse.svg)](https://hub.docker.com/r/cyversevice/shiny-verse)  |  [![](https://img.shields.io/docker/automated/cyversevice/shiny-verse.svg)](https://hub.docker.com/r/cyversevice/shiny-verse/builds)

# Instructions

## Run this Docker image locally or on a Virtual Machine

To run the container, you must first pull from DockerHub

```
docker pull cyversevice/shiny-verse:latest
```

A shiny server should be running on your localhost port `:3838` 

## Build your own Docker container and deploy on CyVerse VICE

This container is intended to run on the CyVerse data science workbench, called [VICE](https://cyverse-visual-interactive-computing-environment.readthedocs-hosted.com/en/latest/index.html). 

Unless you plan on making changes to this container, you should use the existing launch button above. 

###### Developer notes

To build your own container with a Dockerfile and additional dependencies, pull the pre-built image from DockerHub:

```
FROM cyversevice/shiny-verse:latest
```


Shiny requires an application to be added to the tool before it is run. You can add your shiny app installation when the container is built, 

Follow the instructions in the [VICE manual for integrating your own tools and apps](https://cyverse-visual-interactive-computing-environment.readthedocs-hosted.com/en/latest/developer_guide/building.html).
