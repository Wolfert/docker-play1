# The Play 1 web framework in Docker

Play 1 Docker image for development, based on the OpenJDK Docker images. 

The images run `play` as the user `play` with a home directory at `/home/play` so
to run an application in `app_directory` on your local machine:

```
docker run --mount type=bind,src=app_directory,target=/home/play/myapp play1 run /home/play/myapp
```
