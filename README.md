# Web Server Setup with Apache and Let's Encrypt

This repository contains the configuration files and documentation for setting up a web server using Apache and securing it with an SSL certificate from Let's Encrypt.

## Prerequisites

Before following this guide, ensure that you have:

- A registered domain name (Let's Encrypt certificates require a domain name, not an IP address).
- A server running Apache on Ubuntu (or a similar Linux distribution).
- SSH access to the server.

## Public IP Address

This server's public IP address is: 3.87.17.54


## Steps to Run Your Web Server

### 1. **Install Apache**

```bash
sudo apt update
sudo apt install apache2
```

### 2. **Install Certbot for SSL**
```sudo apt install certbot python3-certbot-apache```

### 3. **Obtain SSL Certificate**
```sudo certbot --apache```

### 4. **Verify SSL**
Once completed, your site should be available at https://yourdomain.com.

### 5. **Edit webSite HTML**
To update the HTML content of your site, edit the index.html file:
```sudo nano /var/www/html/index.html```

### 6. **Restart Apache**
If you make changes to the configuration, restart Apache:
```sudo systemctl restart apache2```





