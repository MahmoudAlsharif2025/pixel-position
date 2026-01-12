# Pixel Position – Docker & GitHub Assignment

## Student Information
- Name: Mahmoud Alsharif
- Project Name: Pixel Position
- Course: Operating Systems Lab
- Assignment: Docker & GitHub Basics

---

## Project Description
**Pixel Position** is a Laravel-based web application.  
This project was developed as part of the Operating Systems Lab assignment to demonstrate the practical use of **GitHub for version control** and **Docker for containerizing and running a web application**.

The application was successfully built and executed inside a Docker container using **GitHub Codespaces**.

---

## Technologies Used
- PHP (Laravel)
- Apache Web Server
- Docker
- Git & GitHub
- GitHub Codespaces
- Visual Studio Code (VS Code)

---

## How to Run the Project Using Docker

### Step 1: Verify Git and Docker Installation
Before starting the deployment process, Git and Docker were verified using the following commands:

git --version
docker --version

Step 2: Clone the Repository
The project repository was cloned from GitHub using:


git clone https://github.com/MahmoudAlsharif2025/pixel-position.git
cd pixel-position

Step 3: Dockerfile
A Dockerfile was created to configure the PHP and Apache environment and prepare the Laravel application to run inside a Docker container.

Step 4: Build Docker Image
After creating the Dockerfile, the Docker image was built using:

docker build -t pixel-position .


Step 5: Run Docker Container
The Docker container was started using the following command:

docker run -d -p 8080:80 --name pixel-position pixel-position
To verify that the container is running:


docker ps
Application Running Successfully
After running the container, the application was accessed through the browser and worked correctly.
The Pixel Position web interface appeared successfully, confirming that the application is running inside Docker.

All required screenshots for the assignment are available in:


docs/screenshots/
Production URL
When running the project using GitHub Codespaces, the application can be accessed using a forwarded port URL generated automatically by Codespaces, for example:


https://zany-bassoon-pj6rgvpqqvvgf6p7j-8080.app.github.dev
Note:
The production URL is generated automatically by GitHub Codespaces and may change or become unavailable after stopping or restarting the Codespace.
This behavior is expected and does not indicate an issue with the Docker configuration or the project setup.

GitHub Repository Link
The full source code of the project is available at:

https://github.com/MahmoudAlsharif2025/pixel-position