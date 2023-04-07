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

This command will show the list of available Docker images on your system, including the one you just created.

## Creating a Docker Container from the Fides Image
  
  1. ### Using ```docker run <image_name>```
