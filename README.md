# docker-ffmpeg
Docker image definition with compiled ffmpeg

# Pulling docker image from docker hub
1. Ensure you have [docker](https://www.docker.com) installed
2. Type: `docker pull jcenzano/ffmpeg`

# Creating the docker image locally (optional)
1. Ensure you have docker [docker](https://www.docker.com) and make installed
2. Type `make`

# Testing the image
1. You can test the image with this command (you should see ffmpeg help):
```
docker run --rm -it jcenzano/ffmpeg
```
