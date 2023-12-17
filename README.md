
#  build and Run in background mode  (-d) 
docker-compose up -d --build 

# Build the Docker image:
docker build -t nodejs-image .

# Run the app container:
docker run -d --name nodejs-app -p 3001:3000 nodejs-image

