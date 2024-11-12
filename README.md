
# Python Project - Hello World

This is a simple Python project that prints "Hello World" to the console.

## Technologies Needed

- Python 3.11 or higher
- Docker (to run the project in a containerized environment)
- Visual Studio Code (optional, for better Python development experience)


## Here’s the Dockerfile used and explained :

| **Step**                       | **Description**                                                                                             |
|---------------------------------|-------------------------------------------------------------------------------------------------------------|
| `FROM python:3.11`              | Pull the official Python 3.11 image from Docker Hub.                                                         |
| `WORKDIR /app`                  | Set the working directory inside the container to `/app`.                                                   |
| `COPY ProyectoPython.py /app/ProyectoPython.py` | Copy the Python script (`ProyectoPython.py`) into the container's `/app` directory.        |
| `CMD ["python", "ProyectoPython.py"]` | Run the Python script when the container starts.                                                            |


## Building the Docker Image 
If you prefer to build the Docker image, run this command.

1. **Build the Docker image:**
   
```bash
docker build -t imgpython .
 ```

## Push the image to Docker Hub
To push the image to your own Docker Hub account, follow these steps.

1. **Tag the image:**

    ```bash
    docker tag imgpython jessjoha/imgpython:latest
    ``` 
2. **Push the image to Docker Hub:**
   
    ```bash
    docker push jessjoha/imgpython:latest
    ``` 

### Pull the image from Docker Hub:

```bash
docker pull jessjoha/imgpython
```

## Link to the Docker Hub image:

https://hub.docker.com/r/jessjoha/imgpython

