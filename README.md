# docker-ffmpeg
Docker image definition with compiled ffmpeg

# Pulling docker image from docker hub
1. Ensure you have [docker](https://www.docker.com) installed
2. Type: `docker pull jcenzano/docker-ffmpeg`

# Creating the docker image locally (optional)
1. Ensure you have docker [docker](https://www.docker.com) and make installed
2. Type `make`

# Testing the image
1. You can test the image with this command (you should see ffmpeg help):
```
docker run --rm -it jcenzano/docker-ffmpeg
```

# Using the image
You can call ffmpeg docker like you call the local command, just adding the ffmpeg parameters at the end of the docker run call, synchronous example:
```
docker run --rm -it jcenzano/docker-ffmpeg -i test-input.flv -f mpgts test-out.ts
```
You can also running it in background (daemon) with `-d`:
```
docker run --rm -itd jcenzano/docker-ffmpeg -i test-input.flv -f mpgts test-out.ts
```