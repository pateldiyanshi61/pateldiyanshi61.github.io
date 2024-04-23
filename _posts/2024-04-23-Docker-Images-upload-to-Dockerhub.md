---
title: "Docker Three Tier Architecture"
date: 2024-04-23 00:00:00 +0800
categories: [Docker Three Tier Architecture]
tag: [Docker Three Tier Architecture]

---

# Three-Tier Application Deployment using Dockerfile

We'll outline the steps for Three-Tier Application Deployment using Dockerfile. Certainly! Here are the steps we'll be following:

# Prerequisites

Before you begin, ensure that you have the following installed:                                                
    -Docker

# Project Structure

# backend: 
Node.js application serving as the backend.                                                                 
# frontend:  
React.js application for the frontend.                                                                    
# mysql: 
Dockerfile and configurations for the MySQL database.

# Dockerfile(Backend)                                                                                               
![alt text](/images/10.png )

# Dockerfile(Frontend)
![alt text](/images/8.png)                                                                                        

# Dockerfile(Database)                        
![alt text](/images/9.png )

# Deployment Steps

# 1.Create Network                                                                                                 
a. Navigate to the project directory
![alt text](/images/11.png )

# 2.MySQL Database:                                                                                         
a. Navigate to the mysql directory                                                                       
b. Build the MySQL Docker image:                                                                                   
![alt text](/images/12.png )

c. Run the MySQL container:
![alt text](/images/13.png )

d. Access the MySQL container:
![alt text](/images/14.png )

e. Inside the container, create tables for the database:
![alt text](/images/15.png )
![alt text](/images/16.png )

# 3.Backend Application:                                                                                     
a. Navigate to the backend directory.                                                                            
b. Build the backend Docker image:                                                                                  
![alt text](/images/17.png )

c. Run the backend container:
![alt text](/images/18.png )

# 4.Frontend Application:                                                                                     
a. Navigate to the frontend directory.                                                                            
b. Build the frontend Docker image:                                                                                  
![alt text](/images/19.png )

c. Run the backend container:
![alt text](/images/20.png )

# 5.Access the Application:                                                                                        
Open your favorite browser and visit http://localhost:80. Enjoy exploring the MERN stack application!
![alt text](/images/21.png )

# 6.Upload images to Docker Hub                                                                                      
a. Login into your docker hub account.                                                                              
b. For pushing the images to docker hub first you need to create repository.                                     
    i. Select the Create Repository button.                                                                      
    ii. For the repository name, use 21bcp368-blogpost. Make sure the Visibility is Public.
    ![Create Repository](/images/22.png )                                                                            
    iii. Select Create. Now the repository is successfully created.
    ![Repository created](/images/23.png )                                                                          
c. Now open the Command Prompt                                                                                  
d. Now login into your Docker Hub account using Command Line.                                                       
Command: docker login                                                                                              
e. In the command line, run the docker push command that you see on Docker Hub.
Command: docker push diyanshipatel61/21bcp368:tagname                                                             
![Push Images](/images/24.png )
![Push Images](/images/25.png )
![Push Images](/images/26.png )
f. Docker images are now successfully uploaded to repository.                                               
![Images](/images/27.png ) 







    



