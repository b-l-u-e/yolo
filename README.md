# Create a Basic Microservice

## Objective: Build ecommerce full stack application using docker-compose

### Set up

1: Fork and clone this [repo](https://github.com/Vinge1718/yolo)

2: Add Dockerfile to /client and /backend

3: Add docker-compose.yml to home directory ./

4: Create an account in [dockerhub](https://hub.docker.com/)

5: Create repository in dockerhub

6: Type this in your terminal: `docker tag node:13.12.0-alpine3.10 winniegitau/yolo:1.0.0`

7: After the above command add this: `docker push winniegitau/yolo:1.0.0` to push image to dockerhub


## How to deploy MERN Stack on Google Kubernetes Engine(GKE)

GKE is GCP managed Kubernetes solution that lets you run and manage containerized applications in the cloud.

## Objectives 

1: Dockerize the app and push the images to Google container registry

2: Run the app on GCP GKE

3: Build the kubernetes cluster on GCP GKE

4: Access  clusters from outside

5: Configure Kubectl with GKE Cluster

## To set up the MongoDB need 3 things; A StorageClass, A Headless Service and StatefulSet

The Storage class tells Kubernetes what kind of storage to use for the database nodes. On Google Cloud Platform storage choices are SSDs and hard disks

Headless Service doesnt allocate IP address or forward traffic. When combined with statefulSets they can give you unique DNS addresses that let you directly access the pods

