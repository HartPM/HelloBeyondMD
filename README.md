Prompt:
Make a simple page using HTML, CSS, and/or javascript that displays “Hello BeyondMD!“, and then dockerize it. It must run using docker-compose.


Repro Steps:
1. cd into the directory you want to clone the project to.
2. $ git clone https://github.com/HartPM/HelloBeyondMD
3. $ docker-compose up -d
4. Open http://localhost:3000/ in a web browser.

_________________________________________

Steps followed to dockerize this project:

- To create a Docker image and container
1. Create Dockerfile
2. Start Docker
3. Build docker image 
- $ docker build -t hello-beyondmd . 
4. Create the container 
- $ docker run -d -p 80:80 22614bb65279   
5. Confirm the container is running
- $ docker ps
6. Navigate to localhost:80 on a web browser
7. To stop
- docker stop NAMES (sub in local NAME)

_________________________________________

- To use with Docker Compose
1. Create docker-compose.yml
2. Start Docker
3. Define services
4. Check .yml file for errors
- $ docker-compose config
5. Run docker-compose.yml
- $ docker-compose up -d
