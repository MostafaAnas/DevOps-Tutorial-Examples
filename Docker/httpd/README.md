Q- 
- Create static html file
- Write Dockerfile to build image based on httpd to host the html file and 
specify the following 
- Copy the html file. 
- Copy a new configuration file to listen on port 9999 instead of 80 
- Open the port 9999 in the container 
- Add environment variable CONTAINER with value docker. 
- Add startup command to echo the variable 

```
docker build -f Dockerfile -t custom-httpd .

docker run -p 9090:9999 custom-httpd 

```