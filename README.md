Task 6 — Automated Strapi Deployment using GitHub Actions and Terraform
Overview

This project demonstrates how to automate the deployment of a Strapi application using Docker, Terraform, and GitHub Actions on AWS EC2.

A prebuilt Docker image is pulled from Docker Hub and deployed automatically on an EC2 instance using Terraform. The deployment is triggered through a GitHub Actions workflow.

Architecture

GitHub Actions triggers deployment

Terraform provisions AWS infrastructure

EC2 installs Docker

Docker pulls Strapi image

Application runs and is accessible via public IP

Tech Stack

AWS EC2

Terraform

Docker

GitHub Actions

Strapi CMS

Project Structure
terraform/
  main.tf
  variables.tf
  outputs.tf

.github/workflows/
  terraform.yml

README.md
Deployment Workflow

Push code to GitHub.

Run the GitHub Actions workflow manually.

Terraform creates EC2 instance.

Docker installs and runs Strapi container.

Access application via public IP.

Docker Image

Docker image used:
namitagrawal/strapi-app

How to Deploy

Go to:
GitHub → Actions → Deploy with Terraform → Run workflow

Verification

After deployment:

Check EC2 instance is running

Open public IP in browser

Confirm Strapi setup page loads

Cleanup

Terminate EC2 instance after testing to avoid charges.

Learning Outcomes

Learned infrastructure automation using Terraform

Implemented CI/CD pipeline with GitHub Actions

Deployed containerized application on AWS

Managed cloud resources lifecycle

Author

Namit Agrawal
