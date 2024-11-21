Simple To-Do App

A basic To-Do List application built using Node.js and Express. This app allows users to add and view tasks.

Features

Add new tasks
View existing tasks
Simple and intuitive interface
Technologies Used

Node.js
Express
EJS (Embedded JavaScript templating)
Body-parser
Setup Instructions

Prerequisites

Make sure you have Node.js and npm installed on your local machine. You can download it from Node.js official website.

Running Locally

Clone the repository:

git clone https://github.com/Priyanka544469/Task1-Cloud_Ambassadors.git

cd todo-app

Install the dependencies:

npm install

Run the application:

node app.js

Open your web browser and navigate to http://localhost:3000 to access the app.

Deployment on AWS EC2

Step 1: Launch an EC2 Instance

Log in to the AWS Management Console.
Navigate to the EC2 Dashboard.
Click on Launch Instance.
Choose the Amazon Machine Image (AMI) (e.g., Ubuntu Server).
Choose an Instance Type (e.g., t2.micro for the Free Tier).
Configure Instance Details, Storage, and Tags as needed.
Configure Security Group:
Add an inbound rule to allow HTTP (port 80) or your app's port (e.g., 3000).
Launch the instance.
Step 2: Connect to Your Instance

Once the instance is running, connect via SSH: bash ssh -i "Jagan.pem" ubuntu@ec2-18-236-169-157.us-west-2.compute.amazonaws.com
Step 3: Install Node.js

Update package lists: bash sudo apt update

Install Node.js and npm: bash sudo apt install -y nodejs npm

Step 4: Deploy Your Application
Clone your GitHub repository on the EC2 instance: bash git clone https://github.com/pavan5779/Task-1_Cloud_Ambassadors.git cd todo-app

Install the dependencies: bash npm install

Run the application (use sudo to run on port 80): bash sudo node app.js

Step 5: Access the Application

Open your web browser and navigate to http://<your-ec2-public-ip> or http://<your-ec2-public-ip>:3000 (depending on the port you exposed) to access the To-Do List application.

URL for Public Access

Your deployed app can be accessed (http://18.236.192.223:3000/)

Conclusion

This To-Do List application serves as a simple example of deploying a web application using Node.js and Express on AWS EC2. Feel free to enhance and modify it according to your needs!
