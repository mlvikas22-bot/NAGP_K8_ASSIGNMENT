# Employee API on Amazon EKS

## Code Repository

GitHub Repository:
https://github.com/mlvikas22-bot/NAGP_Code

## Docker Images

Employee API:
https://hub.docker.com/repository/docker/vicky2609/employee-api/tags

## Application URL

http://k8s-nagp-employee-a8eafecad2-2028196337.us-east-1.elb.amazonaws.com

## Solution Overview

This project implements a two-tier application deployed on Amazon EKS.

Frontend/API Tier:

* Flask REST API
* Kubernetes Deployment
* 4 replicas
* Horizontal Pod Autoscaler

Backend Tier:

* MySQL StatefulSet
* Persistent EBS Storage
* Database initialization using ConfigMap mounted SQL scripts

Infrastructure:

* Amazon EKS
* AWS Load Balancer Controller
* Application Load Balancer
* EBS CSI Driver
* ConfigMaps
* Secrets
* Ingress
* HPA

## Kubernetes Objects Used

* Namespace
* Deployment
* StatefulSet
* Service
* Ingress
* ConfigMap
* Secret
* HorizontalPodAutoscaler
* PersistentVolumeClaim
* StorageClass

## Demonstrated Capabilities

* Deployment Strategy (Rolling Update)
* Self Healing
* Persistence
* Horizontal Pod Autoscaling
* High Availability
* Secure Configuration Management

## Video Recording

https://nagarro-my.sharepoint.com/:v:/p/vikas_l/IQDKflZv0oJYRa8OhrDpl2AQAQazGxuXOPdpBheO4IcQHxI?e=gLJJcz

## Cleanup

eksctl delete cluster --name nagp-assignment --region us-east-1
