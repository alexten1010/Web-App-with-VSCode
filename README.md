# Web App with VSCode

## Web App with VSCode is a project designed to demonstrate how to deploy and manage a Java-based web application using AWS resources and Visual Studio Code (VSCode). This project showcases practical steps for configuring cloud infrastructure, setting up development tools, and deploying web applications in a secure and efficient manner.



## Features

Cloud Deployment: Launch and configure an AWS EC2 instance to host the application.

Java Web App: Build and deploy a Java-based web application using Apache Maven.

Remote Development: Use the Remote - SSH extension in VSCode for seamless development on the cloud.

Security: Configure SSH and key pair authentication for secure server access.

Efficient Workflow: Leverage VSCode's file explorer and Maven commands for streamlined development.

## Setup and Installation

Launch an EC2 Instance:

Open the AWS Management Console.

Launch an EC2 instance and configure it with the necessary security group and key pair.

Configure VSCode:

Install the Remote - SSH extension in VSCode.

Connect to the EC2 instance using the .pem key file for authentication.

Install Apache Maven and Amazon Corretto:

Use Maven to manage dependencies and build the Java application.

Install Amazon Corretto 8 to run Java commands on the EC2 instance.

Deploy the Web Application:

Generate a Java web application using Maven.

Edit the index.jsp file to customize the application’s front end.

Deploy the application files to the server.

## Usage

Access the EC2 Instance:
ssh -i ~/.ssh/vscode.pem ec2-user@<EC2_PUBLIC_IP>

Run the Application:

Start the web application server.

Access the application via the EC2 public IP in your browser.

Manage Files with VSCode:

Use VSCode’s file explorer to view and edit the project files directly on the EC2 instance.
Use the following command to establish an SSH connection:

## Example Commands

Update Key Permissions:

chmod 400 ~/.ssh/vscode.pem

Connect to EC2 via SSH:

ssh -i ~/.ssh/vscode.pem ec2-user@<EC2_PUBLIC_IP>

Run Maven Build:

mvn clean install

