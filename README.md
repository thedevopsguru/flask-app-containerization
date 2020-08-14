# flask-app-containerization
For flask app containerazation

Build image
docker build -t myapp:v1.0 .

Run redis container
docker run -d redis:latest

#Link Redis and application container.
docker run -d -p 5000:5000 --link redis myapp:v1.0 
