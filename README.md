#This samples used to create a web app.
it build by mvn clean install
Then it will generate a war file and copy to docker folder
The docker folder finally has two files one is Dockerfile the other one is the war file.
Then run the docker build command

docker build –t registry.ng.bluemix.net/davidchow/dockerwebtest:1.0 .
docker push registry.ng.bluemix.net/davidchow/dockerwebtest:1.0

#deploy to cloud as following
cf login
cf ic login
cf ic run --name david_web registry.ng.bluemix.net/davidchow/image_name:1.0
cf ic ip list

Then bluemix should has a Docker images.
Create a Docker container on the bluemix console panel.




