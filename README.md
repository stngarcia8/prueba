# ![Jansten](https://www.jansten.com/)Api ![License](https://img.shields.io/badge/license-MIT-blue.svg) [![Pull request](https://img.shields.io/badge/Pull%20request-PR-blue)](https://bitbucket.org/inblind/janstenapi/pull-requests/)  

Api Rest developed with Node.js, Express Framework and MongoDB technology, provides support to the activities generated by users from the JanstenApp front-end application.
_ _ _ _ _  

## Requirements
To run JanstenApi, you need to have the following software installed on your computer:
- [Node.js](https://nodejs.org/en/) (version 15.0.1 or higher)
- [Git](https://git-scm.com/downloads)  
_ _ _ _ _  

## Getting Started
- From a command line, create a folder and then clone the repository
```bash
    mkdir jansten
    git clone git@bitbucket.org:inblind/janstenapi.git
```
- Go to the folder generated by cloning the repository
```bash
    cd janstenapi
```
- To install the project dependencies, execute
```bash
    npm install
``` 
- To execute development environment of JanstenApi, execute
```bash
    npm start
```
- Alternatively you can use **nodemon** for update api in real time, in the root folder, execute
```bash
    # to install nodemon
    npm install nodemon

    # to execute nodemon
    nodemon ./src/app.js
```
_ _ _ _ _  

## Running test
Open a command line in the root folder and execute:
```bash
npm test
```
_ _ _ _ _   

## Deploy Heroku test ![Heroku](https://img.shields.io/badge/Heroku-%20-yellowgreen)
* 1- heroku login (open browser and check if have correct heroku login)
* 2- heroku git:remote -a janstenapi (check if have correct repo jansten in heroku)
* 3- git push heroku development:master  
_ _ _ _ _   

## Api documentation [![Swagger](https://img.shields.io/badge/Swagger-2.0-yellow)](http://localhost:3000/api-docs/)
- To generate api documentation, open a command line in the root folder and execute:
```bash 
    npm run apidoc
```
- You can view the documentation at http://localhost:3000/api-docs/
_ _ _ _ _   

## Static code analysis [![Sonarqube](https://img.shields.io/badge/Sonarqube-8.9.0--community-green)](http://localhost:9000)
To run the code analysis, first you need to install [Docker](https://www.docker.com/), once installed, follow the steps below:

1. Download sonarqube image from command line
```bash
    docker pull sonarqube:8.9.0-community
```

2. Create a sonarqube container
```bash
    docker run -d --name jansten_sq -p 9000:9000 sonarqube:8.9.0-community
```

3. Verify that Sonarqube is running at the following url http://localhost:9000, login with the credentials (user admin, password admin) and change the password to admin1

4. Open a command line in the root folder and execute
```bash
    npm run sonar
```
_ _ _ _ _   

## Authors
- Rumina Morales 
- Rafael Montero  
_ _ _ _ _   

## License ![License](https://img.shields.io/badge/license-MIT-blue.svg)
Jansten use the MIT License (MIT)

_ _ _ _ _   
## Copyright
?? 2020-2021 [Jansten](https://www.jansten.com/)
