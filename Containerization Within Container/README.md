# Containerization Within Container

![](images/docker-in-docker.png)

# How it is Different?
The advantage of using this apprach is that we can easily ship this complete project to where ever we want to run it. I have created a Jenkins-image using DOCKERFILE so that all my work will be saved into this and it won't effect my project.

# How to Launch this Project?
As a pre-requisites of this Project docker must be installed in your system and nothing else required. Run the Following commands in your terminal to launch this project.<br>
1. <code>docker pull alex43/jenkins-os:v1.0</code><br><br>
2. <code>docker run -dit -p 1234:8080 -v /:/host -v /var/run/docker.sock:/var/run/docker.sock --name automation_project alex43/jenkins-os:v1.0</code><br><br>
3. <code>Your_IP:1234</code>, Enter your Ip with port specified in browser after running container successfully.

