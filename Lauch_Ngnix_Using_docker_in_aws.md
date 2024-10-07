# Deploying NGINX with Docker on AWS

## Overview

This project demonstrates how to deploy an NGINX web server using Docker on AWS. By leveraging Docker, we can create a scalable and portable web server environment.

## Prerequisites

- An AWS account
- EC2 instance with a compatible OS (e.g., Amazon Linux)
- Basic understanding of Docker and AWS

## Steps to Deploy NGINX

### 1. Install Docker

First, install Docker on your EC2 instance:

```bash
yum install docker
```

### 2. Start Docker Service

Next, start the Docker service:

```bash
systemctl start docker
```

### 3. Verify Docker Status

Check the status of Docker to ensure it’s running:

```bash
systemctl status docker
```

### 4. Pull the NGINX Image

Download the NGINX Docker image:

```bash
docker pull nginx
```

### 5. Verify Available Docker Images

List all available Docker images to confirm the NGINX image is downloaded:

```bash
docker images
```

### 6. Run the NGINX Container

Now, run the NGINX container:

```bash
docker run nginx
```

## Interacting with the NGINX Instance (open same instance)

## Once the NGINX container is running, you can perform the following commands:

### 1. Check Running Containers

To see the currently running containers, use:

```bash
docker ps   # This will display the list of running containers along with their names and IDs.
```

### 2. Inspect the NGINX Container

Inspect the container for details:

```bash
docker inspect <container_name>
```

### 3. Test Connectivity

Test the NGINX server using curl (replace <your_ip_address> with your instance's public IP):

```bash
curl <your_ip_address>
```

### 4. Stop the NGINX Container

To stop the running container:

```bash
docker stop <container_name>
```

### 5. Check Container Status

You can verify the status of running containers again:

```bash
docker ps
```

### 6. List All Containers

To view all containers (including stopped ones):

```bash
docker ps -a
```

### 7. View Command History

To see the history of commands run in the terminal:

```bash
history
```

# Conclusion
By following these steps, you can successfully deploy and manage an NGINX web server using Docker on AWS. 


## Feel free to modify any sections as needed! This format provides a clear and professional presentation of your project.














