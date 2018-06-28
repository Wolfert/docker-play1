# Dockerized Play 1

A Dockerized [Play 1 web framework](https://github.com/playframework/play1) for development, based on the OpenJDK Docker images. 

The images run `play` as the user `play` with a home directory at `/home/play` so
to run an application in `app_directory` on your local machine:

```
docker run --mount type=bind,src=app_directory,target=/home/play/myapp play1 run /home/play/myapp
```
