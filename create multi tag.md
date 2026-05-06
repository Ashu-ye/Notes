mkdir mytask

cd mytask

nano Dockerfile
 (inside that docker file )
FROM ubuntu:22.04

RUN echo "Hello from my image"

CMD ["echo", "container is running"]

(save and quit  :wq)

docker build -t myimage:v1 .

docker tag muimage:v1 myimage:v2

docker tag muimage:v1 myimage:v3

docker image | grep myimage

docker rmi myimage:v2

docker image | grep myimage
