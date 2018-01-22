# jnrstud-minimal

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/lsetiawan/jnrstud-minimal/master)

This Repo contains the Dockerfile for [lsetiawan/jnrstud-minimal](https://hub.docker.com/r/lsetiawan/jnrstud-minimal/).

This image builds from [rocker/geospatial:3.4.3](https://hub.docker.com/r/rocker/geospatial/). The build commands are a compilation between [jupyter base-notebook](https://github.com/jupyter/docker-stacks/blob/8e15d329f1e9aafb54a90c5cc00853d42a9db68f/base-notebook/Dockerfile) and [rocker binder](https://github.com/rocker-org/binder/blob/master/3.4.3/Dockerfile)

To run the Docker image, just simply place the command below in your terminal:
```bash
docker run --name jnrstud -d -p 8888:8888 lsetiawan/jnrstud-minimal:latest
```
Once the image is pulled and ran, you should be able to type `localhost:8888` in your browser. This will redirect you to a jupyter notebook server.

**This Docker image is driven by the IOOS Biological Data Training Workshop. It serves as the baseline image that has both Jupyter Notebook and RStudio to be deployed in a JupyterHub Instance.**
