# Docker Compose Deployment for Nginx and PHP

## Description

This Docker Compose configuration sets up a deployment environment for Nginx and PHP (LEMP) using separate containers. Nginx serves as the web server, while PHP-FPM handles PHP processing.

## Prerequisites

Before you begin, ensure you have Docker and Docker Compose installed on your system.

## Usage

1. Clone this repository to your local machine:

   git clone https://github.com/sudosugandh/Lemp-Stack-Docker.git

2. Navigate to the project directory:

   cd Lemp-Stack-Docker

3. Run the following command to start the containers:

   sudo docker-compose up -d

This command will pull the necessary Docker images (Nginx, PHP-FPM, Adminer, and MySQL), create and start the containers in detached mode.

4. Access the deployed services:

    - Nginx: Open your web browser and navigate to http://localhost to access the Nginx web server.
    - Adminer: Access the Adminer database management tool by navigating to http://localhost:8080.

5. To stop and remove the containers, run:
   sudo docker-compose down

# Customization
   - Custom Nginx Configuration: If you have custom Nginx configuration files, place them in the conf.d directory and mount this directory as a volume in the nginx service definition in docker-compose.yml.

   - Custom PHP Configuration: If you need to customize PHP settings, you can create a custom Dockerfile for the PHP service and configure it accordingly. Update the build option in docker-compose.yml to use your custom Dockerfile.

   - Database Configuration: Modify the MySQL service configuration in docker-compose.yml to suit your database requirements.

# Contributing.

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or create a pull request.
    
   


