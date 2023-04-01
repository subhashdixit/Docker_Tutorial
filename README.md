# Docker_Tutorial
This repo has content about Docker

Create virtual environment using below command:
```
Adding virtual env : python -m venv ./venv
Actiavting virtual env : .\venv\Scripts\Activate.ps1
```
Command to build docker image
```
docker build -t welcome-app .
```
Check docker images
```
docker images
```
Run the docker images - Hostname mapping
```
docker run -p 5000:5000 welcome-app
```
Two IPs: 
```
http://172.0.0.1:5000 -- It is wrt localhost and it will run normally
http://172.17.0.2:5000 -- It will not run initially. It is the IP present in the ocntainer. We can access it through our host container thorugh specific port
```
Command to check how many container is running
```
docker ps
```
Command to stop the container
```
docker stop "container_id"
```