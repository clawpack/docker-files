
# Dockerfiles for Clawpack

To build an image give a command like this in this directory:

    $ docker build -t clawpack/v5.7.1_dockerimage -f Dockerfile_v5.7.1 .

To push to [https://hub.docker.com/u/clawpack/dashboard/](dockerhub):

    $ docker login
    $ docker tag clawpack/v5.7.1_dockerimage:latest \
                 clawpack/v5.7.1_dockerimage:release
    $ docker push clawpack/v5.7.1_dockerimage:release

(Requires an account with with push permission.)

## To use an image:

See [the documentation](http://www.clawpack.org/docker_image.html).

