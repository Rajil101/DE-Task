# Pre-requsite #

#Setup linux ubuntu OS on vagrant cloud

>vagrant up

>vagrant ssh

#Created Kubertness Architecture of 2cpu shown in Vagrantfile

#Install Docker & Docker-compose

#clone the repo from github.com on cloud

>git clone https://github.com/cytopia/docker-dvwa.git

#Initiate in repo folder by changing directory

>cd ./docker-dvwa

# docker-dvwa deployment #

#Step 1:Configuration for app

# Configure RECAPTCHA_PRIV_KEY, RECAPTCHA_PUB_KEY 

##Add Recaptcha Private Key, Recaptcha Public Key through google recaptcha genration

#Lable

#Type: V2

#Domain

>dvwa

>localhost

>127.0.0.1


#Step 2: Docker-compose Alteration 

#Add Keys to vagrant cloud environment in docker-compose.yml with explicite ports and version

>Add SITE KEY to the RECAPTCHA_PUB_KEY variable in your .env file

>Add SECRET KEY to the RECAPTCHA_PRIV_KEY variable in your .env file


#Step 3

#Start the Makefile

>make start

#Check the docker container running
>docker ps

#Run the application

>make start -p 8000

OR define in-line in vagrant file with port forwarding.

# Access the application by typing the localhost in browser

![Screenshot 2024-03-27 174622](https://github.com/Rajil101/Accuknox/assets/86475883/d62b69bb-c72b-4fa2-8832-f96ea12e7856)



#Stop the application server

>make stop
