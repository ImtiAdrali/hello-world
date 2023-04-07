# FIDES DEPLOYMENT TO DOCKER


## Creating an Image
```sh
  gradlew buildDocker
```

This task will compile the application, build the Docker image, and tag the image with the name specified in the docker configuration.
