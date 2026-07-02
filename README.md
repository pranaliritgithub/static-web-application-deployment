# Static Application Deployment using (Amazon Linux)

## Introduction

Static Application Deployment on Amazon EC2 using Amazon Linux and Nginx is a simple and efficient way to host websites. In this setup, a virtual server (EC2 instance) runs Amazon Linux, where Nginx is installed to serve static files like HTML, CSS, and JavaScript.
When a user accesses the website, the request travels through the internet to the EC2 instance, and Nginx quickly delivers the content. This approach is lightweight, fast, and cost-effective, making it ideal for hosting static websites such as portfolios, landing pages, and simple web applications.

## Architecture Diagram

![alt text](<Architecture Dia-1.png>)

## Steps:

### 1. Launch EC2 Instance

![alt text](<Screenshot (366).png>)

### 2. Copy Website Files using SCP

![alt text](<Screenshot (367).png>)

### 3. Install NGINX

- sudo yum update 
- sudo yum install nginx -y 
- sudo systemctl start nginx 
- sudo systemctl enable nginx

### 4. Move Files to NGINX Directory

![alt text](<Screenshot (368).png>)

### 5. Restart NGINX

- sudo systemctl restart nginx

### 6. Access Your Website

![alt text](<Screenshot (369).png>)

## Conclusion

This project shows a simple and efficient way to deploy a static website on AWS using EC2 and NGINX. It is fast, secure, and widely used in real-world cloud deployments.