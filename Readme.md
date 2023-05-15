### Docker Steps:
Check the file Dockerfile

### Command to run on cmd:
- docker build -t welcome-app .
- docker images
- docker run -p 5000:5000 welcome-app

### on another cmd:
- docker ps
- docker stop 

### create an account on hub.docker.com (ONLY PUBLIC if free)
##### On cmd:
- docker login
- <username>
- <password>
- docker build -t <username>/welcome-app .
- docker images
- docker tag <old_name> <new_name>

### To push on the Hub repository:
- docker push <username>/<app-name>:latest

### now we can remove or pull the image:
- docker rm -f ...
- docker pull ...

### Let's run the image as a container from hub and check if it is visible on our docker desktop
- docker run -d -p 5000:5000 <username>/welcome-app:latest
