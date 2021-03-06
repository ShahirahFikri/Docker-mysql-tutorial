# Docker-mysql-tutorial
## OPERATING SYSTEMS CSCI 3300 SECTION 1
## TEAM MEMBERS GROUP 5:

* **NURUL SHAHIRAH BINTI AHMAD FIKRI** Matric ID *2013890*
* **NUR ALIA BINTI MUHAMMAD** Matric ID *2010884*
* **AFIEFAH BINTI JAMALULLAIN** Matric ID *2011666*
* **TAMANNI HAYYAN HANI** Matric ID *2020833*

## LECTURER:
*DR. RIZAL BIN MOHD. NOR*

## WHAT DOCKER IS?

Docker is a free and open set of software, delivering, and operating apps. Docker allows to decouple the apps from infrastructure to swiftly release software. We can organise our hardware the same approach we control our programs with Docker. We may drastically minimise the time between writing code and executing it in operation by leveraging Docker's approaches for shipping, testing, and deploying code quickly. 

## HOW DOCKER WORKS

Docker helps to give users a consistent mechanism to run the code. Docker is a container operating system. Containers deploy a server's operating system in the same way as virtual machines virtualize which eliminate the need to handle server hardware directly. Each server has Docker installed, which provides simple commands for building, starting, and stopping containers.

## EXAMPLE OF DOCKER

For example, a website, API, and database must all be linked together. Docker Compose enables us to accomplish just that. We can make a file that specifies how containers are linked to one other. This file can be used to create all of the Dockerfiles for all of our containers in one go.

* **APACHE**

*Run the docker-compose up command in the same directory as the docker-compose.yaml file to start running all of the specified services as Docker containers.*

![Screenshot (1867)](https://user-images.githubusercontent.com/104122185/173180088-f81a00ec-2e68-4370-8d3d-b91c25174fd4.png)

*The Apache httpd Docker image becomes available on port 8080 once this docker-compose up command accomplishes, with the web server hosting files from the folder supplied in the configuration file's volumes section.*

* **SQL**

*Docker Compose lets us provide properties for a service (in this case, MySQL) such as the image to use, ports to expose, volumes to deploy, and environment variables.*

*Here's how we'd utilise docker-compose to achieve the aforementioned capabilities. This should be saved as docker-compose.yaml:*

![Screenshot (1871)](https://user-images.githubusercontent.com/104122185/173181154-8e2e606d-a786-4766-9117-3ff9b66f5548.png)

* **PHP**

*The docker-compose command accepts several options, followed by a command. In this case, you are using -p tests to run the services under the tests project name. The command being used is run, which will execute a one-time command against a service. The --rm option will remove the containers after the command runs. Finally, we are running in the web service phpunit.*

![Screenshot (1873)](https://user-images.githubusercontent.com/104122185/173181624-2f10cfc7-fe03-4830-a6de-1e099b498465.png)

Tutorial of installation starts at [Page 1](page1.md)
