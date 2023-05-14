# Create-a-static-website-using-Nginx
This project will teach you how to set up a static website using the Nginx web server. You will learn how to install Nginx, create a website, and configure Nginx to serve the website

## Requirements

* A Linux distribution
* A text editor

## Instructions

1. Install Nginx.
sudo apt-get install nginx


2. Create a website directory.
mkdir website


3. Create a index.html file in the website directory.
nano website/index.html


In the index.html file, add the following content:
<!DOCTYPE html>
<html>
<head>
<title>My Website</title>
</head>
<body>
<h1>Welcome to my website!</h1>
</body>
</html>


4. Configure Nginx to serve the website.
sudo nano /etc/nginx/sites-available/mywebsite


### In the mywebsite file, add the following content:

server {
listen 80;
server_name mywebsite;
root /var/www/mywebsite;
}


### Save the file and then enable the mywebsite site:
sudo a2ensite mywebsite

### Restart Nginx:
sudo service nginx restart

Now, you can access your website at http://localhost.

### Conclusion
In this project, you learned how to set up a static website using the Nginx web server. You can now use this knowledge to create your own websites.





