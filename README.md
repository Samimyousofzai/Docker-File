# Docker-File
# Steps to deploy your docker file on docker hub 
# Step 1: Create a dockerfile using: 
    mkdir dockerfile cd dockerfile touch dockerfile. 

# Step 2: write the commands in the docker file #to do so use: 
    vim dockerfile
    now click i to insert 
    WRITE the below commands: 
## getting base image ubuntu 

    FROM ubuntu

    MAINTAINER yourname

    RUN apt-get update

    CMD ["echo", "#helloworld! from my first docker image"] 

## To save and exit : esc :wq! enter 

# Step 3: build the image by docker build -
    tag imagename  
## for tags docker build -tag imagename:tag 

# Step 4: after building u can check for the image and also can run it 
    if you run it should print:helloworld! from my first docker image 

# Step 5: deploy on docker hub via: docker login 
    enter username password docker tag imagename dockerhubusername/imagename docker images docker push dockerhubusername/imagename docker logout 
 
# Your image is now pushed on repository of imagename
