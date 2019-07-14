# Miscellaneous Dockerfiles

This repository contains Dockerfiles that are not associated with any particular project:

- [`adamrehn/docker:python`](./docker/python/Dockerfile): extends the Git-equipped variant of the [official Docker-in-Docker base image](https://hub.docker.com/_/docker) by adding Python and the files required to build native Python extensions. This is primarily useful for running [ue4-docker](https://github.com/adamrehn/ue4-docker) inside a container itself, although it's worth noting that you will need to use `--network=host` for the credential endpoint to function correctly when building UE4 container images.
