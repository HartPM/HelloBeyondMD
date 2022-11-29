Make a simple page using HTML, CSS, and/or javascript that displays “Hello BeyondMD!“, and then dockerize it. It must run using docker-compose.

- Repro steps
1. Clone this repo to a local directory
2. Start Docker
3. Build docker image 
- $ docker build -t hello-beyondmd . 
4. Create the container 
- $ docker run -d -p 80:80 22614bb65279   
5. Confirm the container is running
- $ docker ps
6. Navigate to localhost:80 on a web browser
7. To stop
- docker stop <NAMES>