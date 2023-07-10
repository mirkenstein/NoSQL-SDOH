# Docker NoSQL and SDOH Data 
Instructions for launching minimal working NoSQL database and loading CSV data

### Prepare the data
In this example we will work with the SDOH data from AHRQ which can be found here:
[https://www.ahrq.gov/sdoh/data-analytics/sdoh-data.html](https://www.ahrq.gov/sdoh/data-analytics/sdoh-data.html)

Download one of the ZIP Code Data XLS files.

Open the file in Excel and export the Data tab to CSV.
There are instructions for two different databases with their respective front-end components.

Nex we need to install docker and make sure that it is running properly on our computer.

### Install Docker for your operating system. 
Start page: [Docker Desktop](https://www.docker.com/products/docker-desktop/)

 To test your Docker installation try the Hello-World example ad described here
[https://hub.docker.com/_/hello-world](https://hub.docker.com/_/hello-world)
```shell
docker run hello-world
```
You will see an output similar to this one 
```shell
$ docker run hello-world
Unable to find image 'hello-world:latest' locally
latest: Pulling from library/hello-world
719385e32844: Pull complete
Digest: sha256:a13ec89cdf897b3e551bd9f89d499db6ff3a7f44c5b9eb8bca40da20eb4ea1fa
Status: Downloaded newer image for hello-world:latest

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.
```

Next we will install the NoSQL database Elasticsearch together with its dashboard component called Kibana.
[Install Elastic-Kibana and Load Data](./ELK/README.md)

We will also demonstrate another NoSQL database MongoDB and the UI component for interfacing with Mongo called Compass
[Install MongoDB and Load Data](./Mongo/README.md)


