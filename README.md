# Portfolio-project-6
This project explains how to setup kubernetes service using AWS.


**Container Orchestration**
We have 2 ways to orchestrate the containers in AWS, one is ECS and another is EKS. 

*Lets understand the difference between EKS and ECS:*

EKS is based on Kubernetes, an open-source container orchestration platform, while ECS is a proprietary container orchestration service developed by AWS.

EKS can be installed in 2 ways:

			1) eksctl (Fastest way to create EKS)
			2) AWS console and AWS CLI (gives visibility on how each source is created and how they interact with each other)

EKS installation 
		        1) Fargate (AWS manages underlying infrastructure for you)
		        2) managed nodes (AWS manages servers for you but you have more control over the configuration)

   
**Project Overview**
Here we are going to deploy our application using EKS setup by managed nodes. We are going to setup and access our EKS from an EC2-instance.

**What is kubectl**
	                This is a command-line tool for interacting with a Kubernetes cluster. 
	                It communicates with the cluster’s control plane using the Kubernetes API.
	                With kubectl, you can perform various operations like creating, updating, and deleting different Kubernetes resources (pods, services, deployments, etc.)
	                It’s an essential tool for anyone working with Kubernetes.

**aws-iam-authenticator**
	                This is a tool that uses AWS Identity and Access Management (IAM) credentials to authenticate to a Kubernetes cluster. 
	                It allows you to avoid having to manage a separate credential for Kubernetes access. 
	                This tool is particularly useful if you’re an administrator running a Kubernetes cluster on AWS and you want to leverage IAM for access control.

**eksctl**
	                This is a simple command-line tool for creating and managing clusters on Amazon EKS. 
	                It automates many tasks, such as creating a cluster with a single command. 
	                It’s developed by Weaveworks and is the official CLI for Amazon EKS.

**STEPS**

            
                Step 1: Set up an EC2 Instance and launch it in the same region as your EKS cluster.
                
                Step 2: Install kubectl
                
                Step 3: Install aws-iam-authenticator
                
                Step 4: Install eksctl
                
                Step 5: Create EKS using maganed nodes

                Step 6: Deploy your application and expose the same.

                Step 7: Access your application from browser.
