# Mirocservice with for Chat Ollama LLM Project

## Getting Started
1. To build and run sample applications you need to have Maven, JDK22 and Docker. However, the simplest way to start with it is through any IDE like Intellij or Eclipse.
2. First, you have to run require utility services on Docker container, go to `DevOps-Deployment` folder and run the following command: <br/>

    ```bash
    docker-compose up -d
    ```
3. Then you can compile your application with Maven `mvn clean install package` command.
4. Or you can run directly from your IDE by running the main java file.

## Architecture 
Our sample microservices-based system consists of the following modules:
- **Gateway Service** - the main entry point into the system. This is where all incoming requests are routed to the appropriate microservice. Port 8080. [Link](https://github.com/SBMS-Ollama-Clone/Gateway-Service.git)
- **Config Server** - responsible for keeping the configuration of all services in the system. Port 8888. [Link](https://github.com/SBMS-Ollama-Clone/Config-Server.git)
- **Auth Service** - responsible for user authentication and authorization. Port 8888. [Link](https://github.com/SBMS-Ollama-Clone/Auth-Service.git)
- **Chat Service** - responsible for handling chat of users and save in the `chat-service` DB. Port 9990. [Link](https://github.com/SBMS-Ollama-Clone/Chat-Service.git)
- **Content Service** - responsible for handling chat contents and save in the `content-service` DB. Port 9991. [Link](https://github.com/SBMS-Ollama-Clone/Content-Service.git)
- **Setting Service** - responsible for handling user settings and save in the `setting-service` DB. Port 9992. [Link](https://github.com/SBMS-Ollama-Clone/Setting-Service.git)
- **Mail Service** - responsible for sending email to the user when they register. Port 9995. [Link](https://github.com/SBMS-Ollama-Clone/Mail-Service.git)
- **Notification Service** - responsible for sending notification to the user when they CRUD on chat. Port 9996. [Link](https://github.com/SBMS-Ollama-Clone/Notification-Service.git)
- **Hashicorp Consul Discovery Service** - responsible for service discovery and registration. Port 8500. (Using Docker)
- **Next Web UI Ollama** - responsible for frontend exposed to users. [Link](https://github.com/SBMS-Ollama-Clone/NextJS-WebUI-Ollama.git)
- **DevOps Docker** - responsible for DevOps deployment on those services. [Link](https://github.com/SBMS-Ollama-Clone/DevOps-Deployment.git)

## Author
[![Email](https://img.shields.io/badge/Email-Kimleang-blue?style=flat&logo=gmail)](mailto:kimleang.srd@gmail.com)<br/>
[![Website](https://img.shields.io/badge/Website-Kimleang-blue?style=flat&logo=google-chrome)](https://kkimleang.com)<br/>
[![Github](https://img.shields.io/badge/Github-Kimleang-blue?style=flat&logo=github)](https://github.com/KimleangSama)<br/>
[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-Kimleang-blue?style=flat&logo=google-scholar)](https://scholar.google.com/citations?user=j67umTIAAAAJ&hl=en&oi=ao)<br/>

## LICENSE
[![License](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-blue?style=flat&logo=creative-commons)](https://creativecommons.org/licenses/by-nc-sa/4.0/)<br/>
