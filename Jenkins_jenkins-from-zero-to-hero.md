# jenkins-from-zero-to-hero
- https://dxc.udemy.com/course/jenkins-from-zero-to-hero/learn/lecture/19367702#overview
- https://github.com/ricardoandre97/jenkins-resources

## Install Jenkins
- install virtual machine Oracle VM
- instal centos in that
- get the ip from VM 
- install putty for ssh and connect jenkin machine
```
# First add repo to yum config manager
sudo yum install -y yum-utils
sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
# Use added repo to install and start docker
sudo yum install docker-ce docker-ce-cli containerd.io
sudo systemctl start docker
# Optional: Validate by run sample image 
sudo docker run hello-world
```
![image](https://user-images.githubusercontent.com/69948118/223956515-2a68f1c9-0776-49d1-ab64-c352dbc8197f.png)
![image](https://user-images.githubusercontent.com/69948118/223956552-e7a43923-fd11-4293-988c-30e7dc3cea15.png)

- install docker compose
```
#Copy the appropriate docker-compose binary from GitHub
sudo curl -L https://github.com/docker/compose/releases/download/1.22.0/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose

#NOTE: to get the latest version sudo curl -L https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose


#Fix permissions after download
sudo chmod +x /usr/local/bin/docker-compose

#Verify success
docker-compose version
```
- docker pull jenkin image

![image](https://user-images.githubusercontent.com/69948118/223957240-ced1ca7d-b2a6-4660-9944-10df672708f5.png)
![image](https://user-images.githubusercontent.com/69948118/223957465-52fc0e2e-92e5-43c2-a3e0-1c1e19cd0b50.png)

- how to quite from  vi :  hit :  Escape then shift + : then  wq then enter
- create docker-compose.yml for jenkis image run
![image](https://user-images.githubusercontent.com/69948118/223959607-c429cacb-40c1-41d8-bcba-49a3cc55cd70.png)
![image](https://user-images.githubusercontent.com/69948118/223960200-9259383c-aa22-4a11-8cee-a2e5b04b8e0b.png)
![image](https://user-images.githubusercontent.com/69948118/223960235-cf1ff2b2-adef-4f1f-956f-1cbf6622f27c.png)
![image](https://user-images.githubusercontent.com/69948118/223960285-0edd3e42-43a7-46b9-9827-19e47809ad00.png)
- install suggested plugins
- create admin user
- create local DNS 
- C:\Windows\System32\drivers\etc
![image](https://user-images.githubusercontent.com/69948118/223962721-72336c61-f4dc-42c4-bba6-0dbe6588c5ea.png)
![image](https://user-images.githubusercontent.com/69948118/223962782-d61846df-3ac7-4264-8331-0a541f006a62.png)

## Getting started with Jenkins
- Go to inside jenkin container and sh it
```
docker exec -it <container_name_or_id> <shell>
docker exec -it my_container bash

[jenkins@localhost jenkins-data]$ docker exec -ti jenkins bash
ienkins@2006d27ffa83 : /$
```
![image](https://user-images.githubusercontent.com/69948118/223969920-b701abb6-76a2-48eb-ae29-0b5fe0ca4181.png)
![image](https://user-images.githubusercontent.com/69948118/223969954-9581e80b-27e0-44cc-8e68-7006b1a1f314.png)
![image](https://user-images.githubusercontent.com/69948118/223970158-bae5e6d4-51a3-4df8-928f-8d9e7a539928.png)

- Add paramaters for before building your job with paramater 
- Add list parameters "choice parametrs"
![image](https://user-images.githubusercontent.com/69948118/223975308-6dc35ca0-e7b8-4aa1-969e-2c1ca3c7982e.png)
![image](https://user-images.githubusercontent.com/69948118/223975402-bf3a92c6-1787-4fff-b55a-aec61670981c.png)
- Add basic logic and boolean parametrs
![image](https://user-images.githubusercontent.com/69948118/223975981-30a5321d-bb48-4b56-8089-7b84d2302a5e.png)
- copying file from host to container
![image](https://user-images.githubusercontent.com/69948118/223977018-d3a4f01e-4343-40b1-acf2-0fd228aadb76.png)
![image](https://user-images.githubusercontent.com/69948118/223977444-b0b7d4d7-eda3-443a-aada-fea631ae4638.png)

## Jenkins & Docker
- install plugin
![image](https://user-images.githubusercontent.com/69948118/223986781-18897dbd-ae65-48da-b039-76d9189e2a7c.png)

## Jenkins & AWS
- upload mysql db backup into aws s3 using jenkins
```sh
#/bin/bash

DATE=$(date +%H-%M-%S)
BACKUP=db-$DATE.sql

DB_HOST=$1
DB_PASSWORD=$2
DB_NAME=$3
AWS_SECRET=$4
BUCKET_NAME=$5

mysqldump -u root -h $DB_HOST -p$DB_PASSWORD $DB_NAME > /tmp/$BACKUP && \
export AWS_ACCESS_KEY_ID=AKIAJRWZWY3CPV3F3JPQ && \
export AWS_SECRET_ACCESS_KEY=$AWS_SECRET && \
echo "Uploading your $BACKUP backup" && \
aws s3 cp /tmp/db-$DATE.sql s3://$BUCKET_NAME/$BACKUP
```

## Jenkins & Ansible
## Install Ansible
- create docker file for creating image for ansible on top of jenkis running image
```
FROM jenkins/jenkins

USER root

RUN apt-get update && apt-get install python3-pip -y && \
    pip3 install ansible --upgrade

USER jenkins
```



