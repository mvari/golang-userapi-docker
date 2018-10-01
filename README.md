# golang-userapi-docker
Generic API service storing users, built up on Golang using MySQL as data storage.

### Golang UserApi
src/ directory contains the golang api code and the Dockerfile.

### Mysql UserAPI Schema
mysql/ directory contains the DB schema and the Dockerfile.

## How to test the service functionality
curl --header "Content-Type: application/json" --request POST --data '{"name":"test user","age":30}' http://host:8080/user

curl --header "Content-Type: application/json" --request POST --data '{"name":"test user 2","age":40}' http://host:8080/user

curl --header "Content-Type: application/json" http://host:8080/users

curl --header "Content-Type: application/json" http://host:8080/user/1

curl --header "Content-Type: application/json" http://host:8080/user/2
