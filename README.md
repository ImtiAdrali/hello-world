# FIDES DEPLOYMENT TO DOCKER


## Creating an Image
```sh
  # create an image from the application
  gradlew buildDocker
```

This task will compile the application, build the Docker image, and tag the image with the name specified in the docker configuration.

#### Verify that Docker image was created successfully.
```sh
  # verify image 
  docker images
```
