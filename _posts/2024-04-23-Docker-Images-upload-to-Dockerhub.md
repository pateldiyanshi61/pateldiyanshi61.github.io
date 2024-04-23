---
title: "Docker"
date: 2024-04-23 00:00:00 +0800
categories: [Docker]
tag: [Docker]

---

# Upload The Container Images To Docker Hub

We'll outline the steps for uploading Docker container images to Docker Hub.Certainly! Here are the steps we'll be following:

1.Login into your docker hub account.
![alt text](/images/7.png )
2.For pushing the images to docker hub first you need to create repository.
![alt text](/images/7.png )
    a. Select the Create Repository button.
    ![alt text](/images/7.png )
    b. For the repository name, use getting-started. Make sure the Visibility is Public.
    ![Create Repository](/images/2.png )
    ![alt text](/images/7.png )
    c. Select Create. Now the repository is successfully created.
    ![Repository created](/images/6.png )
![alt text](/images/7.png )
3.Now open the Command Prompt
![alt text](/images/7.png )
4.Now login into your Docker Hub account using Command Line.
Command: docker login -u diyanshipatel61
![Login in Docker Hub](/images/3.png )
![alt text](/images/7.png )
5.In the command line, run the docker push command that you see on Docker Hub.
Command: docker push diyanshipatel61/getting-started
![Push Images](/images/5.png )
![alt text](/images/7.png )
6.Docker images are now successfully uploaded to repository.
![Images](/images/4.png )





    



