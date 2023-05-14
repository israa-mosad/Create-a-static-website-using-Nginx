# Create-a-static-website-using-Nginx
This project will teach you how to set up a static website using the Nginx web server. You will learn how to install Nginx, create a website, and configure Nginx to serve the website

## Requirements

* A Linux distribution
* A text editor

## Instructions

### 1. Install Nginx.
sudo apt-get install nginx


### 2. Create a website directory.
mkdir website


### 3. Create a index.html file in the website directory.
nano website/index.html


### In the index.html file, add the following content:
 ![image](https://github.com/israa-mosad/Create-a-static-website-using-Nginx/assets/133568327/00248b3a-aed3-4880-81fe-3e98c9f60877)


### 4. Configure Nginx to serve the website.
sudo nano /etc/nginx/sites-available/mywebsite


### In the mywebsite file, add the following content:

![image](https://github.com/israa-mosad/Create-a-static-website-using-Nginx/assets/133568327/b296111b-8983-4de7-a529-90906714833c)


### Save the file and then enable the mywebsite site:
sudo a2ensite mywebsite

### Restart Nginx:
sudo service nginx restart

Now, you can access your website at http://localhost.

### Conclusion
In this project, you learned how to set up a static website using the Nginx web server. You can now use this knowledge to create your own websites.





