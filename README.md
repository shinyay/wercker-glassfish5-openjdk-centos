# Wecker for GlassFish 5 with OpenJDK 8 on CentOS 7

This Wecker application makes GlassFish 5 runtime environment on CentOS 7.

## Description

GlassFish 5 is the Java Application Server for reference implementation of Java EE 8.
It is built and released weekly as beta edition since Java EE 8 is not official released yet.
So you have to download and install it originally when you use it.

This Wecker application enables you to omit your process and use it easily and quickly.

## Demo

## Features

- GlassFis 5 version is selectable
  - version is defined as enviroment variable
- CentOS version is selectable
  - version is defined as enviroment variable
- Java 8 is pre-installed
  - confired JAVA_HOME and PATH

## Requirement

Wercker account

## Usage

### 1. Edit Repository Information

Edit the following step in wercker.xml.

- USERNAME: Repository User Account Name
- PASSWORD: Repository User Account Password
- DOCKER_IMAGE_NAME: Image name in Repository
- DOCKER_IMAGE_TAG: Image's tag as version
- DOCKER_IMAGE'S_AUTHOR_NAME: Images's author Information

```
- internal/docker-push:
     username: [USERNAME]
     password: [PASSWORD]
     repository: [DOCKER_IMAGE_NAME]
     tag: [DOCKER_IMAGE_TAG]
     author: [DOCKER_IMAGE'S_AUTHOR_NAME]
     cmd: /bin/bash --login
```

### 2. Ceate Application in Wercker

## Installation

doker pull in your repository you pushed.

## Licence

Released under the [MIT license](https://gist.githubusercontent.com/shinyay/56e54ee4c0e22db8211e05e70a63247e/raw/44f0f4de510b4f2b918fad3c91e0845104092bff/LICENSE)

## Author

[shinyay](https://github.com/shinyay)
