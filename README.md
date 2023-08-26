## Django Multi-Application Project with Docker and Nginx Load Balancing
## with Round Robin Algorithm
### Objective
The objective of this project is to demonstrate how to create a multi-application Django project using Docker Compose and set up Nginx for load balancing between the applications. By containerizing the Django applications and utilizing Nginx as a load balancer, this project showcases a scalable and efficient way to manage multiple applications and distribute incoming traffic.

### Description
This project provides a comprehensive example of how to set up multiple Django applications, each running on its own port within Docker containers. The applications are orchestrated using Docker Compose, which simplifies the process of managing and linking the different components. Nginx is then introduced to act as a load balancer, distributing incoming requests across the various Django application instances.

## Technologiews Used
- python
- django
- Docker
- Docker Compose
- Nginx
- git

## Setup
Prerequisites
- Docker and Docker Compose are installed on your system.
## Steps

<details>
<summary><h3>1. Clone the Repository:</h3></summary>

- git clone https://github.com/YounisSaeed/LoadBalance-django-docker-nginx.git
- cd LoadBalance-django-docker-nginx

</details>

<details>
<summary><h3>2. Configure Django Applications:</h3></summary>

Customize each Django application in the project1/ and project2/ directories.
Update project1/requirements.txt and project2/requirements.txt with your application's dependencies.
</details>
<details>
<summary><h3>3. Configure Nginx Load Balancer:</h3></summary>

Modify the nginx/nginx.conf configuration to suit your project's needs.
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
The Nginx load balancer is accessible at http://localhost:8888.
</details>



