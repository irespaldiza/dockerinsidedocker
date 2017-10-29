## Docker iside Docker

This Docker image allows you run Docker inside a Docker container. 
This image of Docker is similar to the official [Docker image](https://github.com/docker-library/docker), generated from Debian instead of alpine linux.
This project has two purposes, on the one hand, constitutes a proof of concept and, on the other, is the basis of other of my images, including my development center. If you want to know more about it, follow the following link: walrus.

---

To run this image you have to expose the Docker socket to your Docker CI container, by bind-mounting it with the flag -v.
~~~ docker run -v /var/run/docker.sock:/var/run/docker.sock \
           -it irespaldiza/dockerinsidedocker
           ~~~
