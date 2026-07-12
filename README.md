# AWS EC2 Static Website

This project demonstrates how to deploy a static HTML website on an AWS EC2 Ubuntu instance using Apache HTTP Server. The website is hosted on a Linux virtual machine and accessed through the EC2 public IP address.

## Tech Stack

- AWS EC2
- Ubuntu
- Apache HTTP Server
- HTML
- Git
- GitHub

## Project Structure

aws-ec2-static-website/
├── index.html
├── README.md
└── screenshots/

## Deployment Steps

Launch an Ubuntu EC2 instance.

Connect to the instance using SSH.

ssh -i <key-pair>.pem ubuntu@<public-ip>

Update the package list.

sudo apt update

Install Apache.

sudo apt install apache2 -y

Copy the website to the Apache document root.

sudo cp index.html /var/www/html/index.html

Verify that Apache is running.

sudo systemctl status apache2

## Access the Application

http://<EC2-Public-IP>

## Repository Contents

- `index.html` – Static website
- `README.md` – Project documentation
- `screenshots/` – Deployment screenshots
