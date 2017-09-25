# docker-amazon-ecr-credential-helper

Yet another repository to build the docker-amazon-ecr-credential-helper? Yes indeed. The reasons why I needed this were:
- having a small docker image based on alpine:edge that would contain the docker-credential-ecr-login binary to use as a base image. In order to minimise size and clutter, I used a build stage and then copied the result in the exported image
- I wanted to build the latest version of the tool (most other images build old versions where it was still the `ecr-login/cmd` package)

So, there you have it.
