
# Dockerfiles for Clawpack

To build an image give a command like this in this directory:

    $ docker build -t clawpack/v5.9.0_dockerimage -f Dockerfile_v5.9.0 .

To push to [https://hub.docker.com/u/clawpack/dashboard/](dockerhub):

    $ docker login
    $ docker tag clawpack/v5.9.0_dockerimage:latest \
                 clawpack/v5.9.0_dockerimage:release
    $ docker push clawpack/v5.9.0_dockerimage:release
    $ docker push clawpack/v5.9.0_dockerimage:latest

(Requires an account with with push permission.)

Note that the `release` version is needed e.g. for [Dockerfiles used 
on mybinder.org](https://mybinder.readthedocs.io/en/latest/tutorials/dockerfile.html),
while the `latest` version allows users to do a
`docker pull` without specifying a version, to get this by default.

## To use an image:

See [the documentation](http://www.clawpack.org/docker_image.html).
