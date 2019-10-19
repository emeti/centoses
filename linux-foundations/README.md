# CentOS docker image for Linux Foundations training

Example Dockerfile allowing to  build a minimal CentOS image suitable for foundation training purposes. 
Based on the main docker image of CentOS 8 with some packages added to enable commands used in the training.

See also comments in the [Dockerfile](./Dockerfile)

You need docker. If not installed see instructions at [https://docs.docker.com/install/](https://docs.docker.com/install/)

You can build the image and then run it as a docker container.

## Building docker image

```
docker build --t  mycentos:0.0.10 -t mycentos:latest .
```
Note that the dot at the end as the last argument of docker build is important. Version 0.0.10 is given as an example.

See the  bash script is provided to capture any customizations. You can execute it from your shell by 
``
``

## Running docker image

```
docker run -it --name <myname> mycentos 
```
Notes: arugments of docker run are positional and it is important that the image name is given as the last argument

If you have built your own imnage with a different name then obviously you need to replace "mycentos" in the docker run  with your assigned name.
 
## Docker survival kit

```
docker build
docker images
docker image rm <imageid>
docker ps
docker ps -a
docker container rm <containerid>
docker run -it <imnagetagname> --name <my-image-nickname>
```
