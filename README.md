
# Dockerfiles for Clawpack

To build an image give a command like this in this directory:

    $ docker build -t clawpack/v5.4.0_dockerimage -f Dockerfile_v5.4.0 .

To push to [https://hub.docker.com/u/clawpack/dashboard/](dockerhub):

    $ docker push clawpack/v5.4.0_dockerimage

(Requires an account with with push permission.)

## To use an image:

See [the documentation](http://www.clawpack.org/docker_image.html).

