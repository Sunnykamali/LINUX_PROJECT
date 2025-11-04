🌐 Hosting and Deploying a Static Website Using Apache Web Server on Linux
📘 Aim of the Project

To host and deploy a static website using the Apache web server on a Linux-based operating system.
The project aims to understand how a web server works, how to configure it to serve static web content, and how to manage logs and permissions in a real-time environment.

⚙️ Performing Tasks

The major tasks performed in this project include:

Installing the Apache HTTP Server

Deploying a pre-built static website (HTML, CSS, and JavaScript)

Testing the website locally and on the local network

Understanding file permissions, configuration directories, log files, and network access

This helps in building a foundational understanding of real-world web hosting environments and server-side management.

🧩 Introduction

A web server is a system that hosts websites and makes them accessible via browsers.
Apache HTTP Server is one of the most popular open-source web servers, known for its reliability, security, and cross-platform support.

In this project, a static website was hosted on a Linux environment using Apache.
It demonstrates how an HTML/CSS/JS-based website can be deployed and accessed using localhost or LAN IP addresses.

The project also emphasizes:

Directory structure of web servers

Permission management

Client-server architecture fundamentals

Hosting a static website means serving HTML, CSS, and JS files directly — ideal for portfolios, landing pages, or documentation websites.

🎯 Objectives

Install and configure Apache web server on Linux

Deploy and host static web content (HTML, CSS, JS)

Understand /var/www/html directory structure

Set and verify permissions for web directories

Manage Apache services (start, stop, enable)

Access hosted website via localhost and LAN IP

Monitor server activity using access and error logs

Gain exposure to server administration and networking

🧰 Tools and Technologies Used
Tool / Technology	Purpose
Linux (Ubuntu)	Operating system for hosting
Apache2	Open-source HTTP server
HTML / CSS / JS	Frontend web technologies
Terminal / CLI	Configuration and management
Web Browser	Testing and viewing hosted site
Network IP	LAN access across devices
🪜 Steps Included
S1) Update System Packages
sudo apt update

S2) Install Apache Web Server
sudo apt install apache2 -y


After installation, Apache runs automatically and creates /var/www/html.

S3) Start and Enable Apache Service
sudo systemctl start apache2
sudo systemctl enable apache2

S4) Check Apache Service Status
sudo systemctl status apache2

S5) Copy Website Files to Web Directory
sudo cp -r /path/to/your/website/* /var/www/html/

S6) Set Directory Permissions
sudo chmod -R 755 /var/www/html
sudo chown -R www-data:www-data /var/www/html

S7) Restart Apache Service
sudo systemctl restart apache2

S8) Check System IP Address
hostname -I

S9) Access the Website

On the same system: http://localhost

On another device (same LAN): http://<system-IP>

S10) Monitor Apache Logs
sudo tail -f /var/log/apache2/access.log
sudo tail -f /var/log/apache2/error.log

🧮 Algorithm / Flow

Start the Linux OS

Update repositories

Install Apache2

Start and enable service

Replace default files with custom website

Set directory permissions

Restart Apache

Find system IP (hostname -I)

Access website via browser

Monitor logs for activity and errors

💻 Code Overview

The hosted website includes:

index.html — Homepage

style.css — Styling

script.js — Interactivity

When Apache receives an HTTP request, it automatically serves index.html from the web root directory (/var/www/html).

No backend processing is involved — making it fast, simple, and secure for static content.

🧾 Terminal Output

Apache installation confirmation

Service status (active and running)

File copy and permission commands executed successfully

IP address retrieved for LAN access

🌍 Browser Output

Website successfully loaded on both:

http://localhost

http://<LAN-IP>

🧠 Conclusion

This project demonstrated the complete process of:

Installing and configuring Apache

Deploying a static website

Managing directories, permissions, and logs

It strengthened understanding of web hosting, client-server communication, and server uptime management.

This forms a strong foundation for future learning in:

DevOps

Cloud Hosting

Backend Server Management

🎓 Learning Outcomes

✅ Learned Apache installation and configuration
✅ Understood static web hosting on Linux
✅ Gained insight into directory structure and permissions
✅ Monitored logs for troubleshooting
✅ Acquired hands-on exposure to basic networking and system admin concepts
