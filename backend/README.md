Backend based on python image  
Git clone on docker host, then change config:  
allowed hosts (ip server), db settings, CORS_ORIGIN_WHITELIST  
  
docker build -t myback backend/  
docker run -it -p 8000:8000 myback  
