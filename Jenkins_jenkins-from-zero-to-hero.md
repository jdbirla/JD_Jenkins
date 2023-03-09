# jenkins-from-zero-to-hero
- https://dxc.udemy.com/course/jenkins-from-zero-to-hero/learn/lecture/19367702#overview
- https://github.com/ricardoandre97/jenkins-resources

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



