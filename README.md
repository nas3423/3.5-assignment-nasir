# 3.5-assignment-zaw

##step-by-step how to create an image until it will be deployed to AWS ECR
- Step 1: Create a ECR repo in the AWS
- Step 2: Make sure that application to be dockerized is in the folder
- Step 3: Build an image using "docker build -t <image name eg. hello-node>
- Step 4: tag an image in ECR repo using " docker tag <image name>:<name tag> <repository_URI>:<image_tag>
        docker tag hello-node:latest <account no>.dkr.ecr.us-east-1.amazonaws.com/nasir-ecr-repo:latest
- Step 5: Ensure to authenticate the Docker client to the registery.
- Step 6: After tagging, push the image to ECR repoby using "docker push <account no>.dkr.ecr.us-east-1.amazonaws.com/nasir-ecr-repo:latest"

- Referenced from zaw
