## docker-kubernetes

This is a repo where I will be committing files while working with docker and kubernetes. The files are hands on practice of Udemy Course (Docker and Kubernetes: A Practical Guide (2022 Edition) by Maximuller


#### Troubleshoot

##### Troubleshoot 1

While restarting ubuntu, docker command gives 'permission error'

`Got permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Get "http://%2Fvar%2Frun%2Fdocker.sock/v1.24/containers/json?all=1": dial unix /var/run/docker.sock: connect: permission denied`

##### Solution:

in `terminal`, run the follwing commands

> `sudo usermod -aG docker tanmoyhalder`
> `sudo chmod 666 /var/run/docker.sock`

then just to check if docker is working fine use the following command

> `docker run hello-world`

##### Troubleshoot 2

To run FastAPI app outside container we need to make sure bot the ports are the ame i.e. 8000

