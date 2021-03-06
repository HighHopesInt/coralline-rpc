# coralline-rpc

## Table of contents
- [Getting Started](#getting-started)
  * [Dependencies](#dependencies)
  * [Installation](#installation)
- [Documentation](#documentation)
  * [Run project](#run-project)
  * [Run in virtualenv](#run-in-virtualenv)
  * [Create Image](#create-image)

## Getting started

### Dependencies
#### This application works in conjunction with:
* https://github.com/HighHopesInt/coralline-dashboard
* https://github.com/Sergei-vb/coralline-components

### Installation
1. [Docker](https://docs.docker.com/install/ "Docker")
2. [Docker compose](https://docs.docker.com/compose/install/ "Docker compose")

## Documentation
### Run project
You need to go to the directory with the Dockerfile of the cloned repository, then:
1. Create Image: ```docker build -t NAME_YOUR_IMAGE .```
2. Enter the parameters of the docker-compose.yml:
   * ```image: ```NAME_YOUR_IMAGE
3. Run Container: ```docker-compose up```

### Run in virtualenv
* You need setup:
  * Supervisor: ```http://supervisord.org/installing.html```
  * Virtualenv: ```https://virtualenv.pypa.io/en/stable/installation/```
  * Python 3.6 ```https://www.python.org/downloads/```

* and run script:
  * ```./start.sh```

* The launch port of the tornado changes in the file "tornado_celery.conf"

### Create image
To create an image, you need a link to the github repository with a Dockerfile, like this: ```https://github.com/Sergeivb/coralline-rpc```