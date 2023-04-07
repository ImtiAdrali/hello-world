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
  
   To create Docker Container from fides image use the below command listed
   
   ```sh
     docker run fides
   ```
    
   This is the most common way to create a container from a docker image. 
   This command starts a new container based on the specific image.
    
  2. ### Using ```docker-compose up``` from the deployment folder
  
    To create a Docker Container from fides image use the below command listed
    ```sh
      docker-compose up
    ```
    Docker Compose is a tool for defining and running multi-container Docker applications. You can create a docker-compose.yml file that 
    specifies the image to use for each service and use the docker-compose up command to start the containers.
