Database based on postgres image  
Allow connection from backend: host myproject myprojectuser 0.0.0.0/0 md5  
Set env vars for db

docker build -t mypostgres database/
docker run -d -p 5432:5432 mypostgres
