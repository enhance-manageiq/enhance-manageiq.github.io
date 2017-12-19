---
layout: post
title: Run ManageIQ using Docker
subtitle: Containerize ManageIQ
author: Akshay Gaikwad
tags: [ManageIQ, Docker, Setup]
---

To test ManageIQ, Docker image for ManageIQ is available. ManageIQ can be run in Docker container. There are also other options like [Public cloud](http://manageiq.org/docs/get-started/cloud) or [Vagrant](http://manageiq.org/docs/get-started/vagrant) to get started with ManageIQ. ManageIQ can run everywhere Docker is available.

First thing, you have to install Docker in your system. Follow instructions in [Docker docs](https://store.docker.com/search?type=edition&offering=community) to install Docker.

Start docker service using

``` $ sudo service docker start ```

### Step 1: Pull Docker image of ManageIQ

``` $ sudo docker pull manageiq/manageiq:fine-3 ```

It will download ManageIQ fine3 image from Docker registry. To see image list, run this

``` $ sudo docker images ls ```

### Stpe 2: Run Docker container

``` $ sudo docker run --privileged -d -p 8443:443 manageiq/manageiq:fine-3 ```

It will run container in detached mode. To see list of running container, execute

``` $ sudo docker ps ```


Now ManageIQ container is up and running at IP address [https://127.0.0.1:8443](https://127.0.0.1:8443)

It has username as *admin* and password is *smartvm*. Get login and explore the world of ManageIQ.
