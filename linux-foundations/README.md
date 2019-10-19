# CentOS docker image for Linux Foundations training

Example Dockerfile which allows buildin CentOS image  with some commands added to get going

See also comments in the [Dockerfile](./Dockerfile)

You need docker. If not installed see instructions 

You can build the image and then run it 

## Building docker image

```
docker build --t  mycentos: -t mycentos:latest .
```
Note that the dot at the end as the last argument of docker build is important

Example bash script is provided to capture any customizations. You can execute it 

## Running docker image

```
docker run -it --name <myname> mycentos 
```
Notes: arugments of docker run are positional, it is important that the image is the last argument

If you have built your own imnage with a different name then replace mycentos with your assigned name.
 
## Docker survival kit

docker build
docker images
docker image rm <imageid>
docker ps
docker ps -a
docker container rm <containerid>
docker run -it <imnagetagname> --name <my-image-nickname>

