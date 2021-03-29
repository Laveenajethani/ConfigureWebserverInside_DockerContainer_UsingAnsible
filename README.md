# Configure Webserver Inside Docker Container

**As we know that by default if we create container using centos image so inside docker container we can not do remote login using SSH but we can enable this feature**

**I have created dockerfile and from this dockerfile I will create my own customize docker image so that we can do SSH login inside the docker container**

In workspace I have created on folder Dockerfile and inside this folder I have Dockerfile .

<img src="Screenshots/file structure.PNG" >

# Dockerfile 

<img src="Screenshots/dockerfile.PNG" >

**Let's build the docker image**

<img src="Screenshots/dockerfile_build.png" >

**I have created ansible playbook docker-host.yml . This playbook do following action:**
- install docker 
- Start docker service 
- Launch container & expose the docker conatiner 
- Reterive docker container IP 
- Inside inventory mentioning docker container IP for further webserver configuration

<img src="Screenshots/docker-host_1.png" >

<img src="Screenshots/docker-host_2.png" >



