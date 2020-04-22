# filehandler
file handler with basic operation to upload and download using api

to run the application follow the below commands.
git clone 'https://github.com/<user>/filehandler.git'
mvn clean test package spring-boot:run
  
Use below curl commands to validate the application.
curl --location --request GET 'http://localhost:8080/health' \
--header 'Content-Type: text/html'

curl --location --request POST 'http://localhost:8080/uploadFile' \
--form 'file=@/Users/<file.ext>'

curl --location --request GET 'http://localhost:8080/downloadFile/<file.ext>'
