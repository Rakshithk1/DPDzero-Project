This is a small project where I created two backend services using:

- Go (Golang)
- Python with Flask

What This Project Does

- Go app runs on port 8001
- Python app runs on port 8002
- NGINX listens on port 8080 and routes traffic:
   /service1/ - Go service
   /service2/ - Python service

So when you open your browser and go to:
 http://localhost:8080/service1/ping - It hits the Go app
 http://localhost:8080/service2/ping - It hits the Python app


Make sure Docker and Docker Compose are installed.

Then run this command in the project folder:

docker-compose up --build

Once this is built, you can check it using docker ps and see if the container is running and once it is running access the above link and check website content if it matches.
