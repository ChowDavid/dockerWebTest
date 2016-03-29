#This samples used to create a web app.
it build by mvn clean install
Then it will generate a war file and copy to docker folder
The docker folder finally has two files one is Dockerfile the other one is the war file.
Then run the docker build command

#deploy the code into bluemix contrainer images
cf login
cf ic login
cf ic build dockerwebtest:1.0 .
cf ic images


#create an contrainer
at bluemix create a new contraner project and run it as example
http://134.168.25.174:9080/dockerWebTest/





