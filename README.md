## Django Multi-Application Project with Docker and Nginx Load Balancing using Least Connections Algorithm

### Objective

The objective of this project is to demonstrate how to create a multi-application Django project using Docker Compose and set up Nginx for load balancing between the applications. By containerizing the Django applications and utilizing Nginx as a load balancer with the Least Connections algorithm, this project showcases a scalable and efficient way to manage multiple applications and distribute incoming traffic effectively.

### Description

This project provides a comprehensive example of how to set up multiple Django applications, each running on its own port within Docker containers. The applications are orchestrated using Docker Compose, which simplifies the process of managing and linking the different components. Nginx is then introduced as a load balancer, configured to distribute incoming requests using the Least Connections algorithm across the various Django application instances.

## Technologies Used

- Python
- Django
- Docker
- Docker Compose
- Nginx
- Git

## Setup

### Prerequisites

- Docker and Docker Compose are installed on your system.

## Steps

<details>
<summary><h3>1. Clone the Repository:</h3></summary>

- git clone -b Least-Connections https://github.com/YounisSaeed/LoadBalance-django-docker-nginx.git
- cd LoadBalance-django-docker-nginx

</details>

<details>
<summary><h3>2. Configure Django Applications:</h3></summary>

Customize each Django application in the project1/ , project2/ and project3 directories.
Update project1/requirements.txt , project2/requirements.txt and project3/requirements.txt with your application's dependencies.
</details>

<details>
<summary><h3>3. Configure Nginx Load Balancer:</h3></summary>

Modify the nginx/nginx.conf configuration to suit your project's needs. Ensure the Least Connections algorithm is correctly configured to balance traffic among the Django applications as needed.
</details>

<details>
<summary><h3>4. Build and Run Containers:</h3></summary>

Run the following command to build and start the containers:

- docker-compose up --build -d

</details>

<details>
<summary><h3>5. Access the Applications:</h3></summary>

Application 1: Access http://localhost:8001
Application 2: Access http://localhost:8002
Application 2: Access http://localhost:8003

The Nginx load balancer, utilizing the Least Connections algorithm, is accessible at http://localhost:8888.


</details>
