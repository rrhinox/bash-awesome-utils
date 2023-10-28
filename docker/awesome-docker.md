# 🐋 My Docker useful and awesome command line for day by day!

## Intro & Documentation

***What is Docker?***

Docker is an open platform for developing, shipping, and running applications. Docker enables you to separate your applications from your infrastructure so you can deliver software quickly. With Docker, you can manage your infrastructure in the same ways you manage your applications. By taking advantage of Docker's methodologies for shipping, testing, and deploying code, you can significantly reduce the delay between writing code and running it in production.



[Docker Overview][dover]

[dover]: https://docs.docker.com/get-started/overview/

[Docker Reference][dref]

[dref]: https://docs.docker.com/reference/

[Docker CLI][cli]

[cli]: https://docs.docker.com/engine/reference/commandline/cli/

[Docker Resources][dr]

[dr]: https://docs.docker.com/get-started/resources/


## Main command 
+ `docker build -t jdk18:1 .` - docker build image from this (".") folder/context of a Dockerfile

+ `docker run -it -d 5b7ea5501286` - run container image in detached mode

+ `docker run --name jdk18 -it -d eaa0a2a` - run container image with name in detached mode

+ `docker exec -it jdk18 bash`

## Example with some context
WIP