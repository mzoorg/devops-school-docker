Multistage build frontend app  
docker build -t myfront_multi frontend/  
docker run -d -p 3000:3000 myfront_multi  

