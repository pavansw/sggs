docker build -t myapp .
docker images
docker run --name=mynodb -d redis
docker ps
docker run -p 5000:5000 -d --link=mynodb:mynodb myapp
