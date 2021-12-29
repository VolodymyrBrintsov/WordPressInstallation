# WordPressInstallation

Install WordPress on given ip address using ansible.

# Installation Process:
1. Installation of DataBase:
    - We send to the server link of MariaDB repository, config file is located in `files` by name `MariaDb.repo`
    - Using `yum` we install the `MariaDB-server` and `MariaDB-client`
    - Using `yum` we install `MySQL-python` package
    - Create DataBase and User and asign all privileges to that user
2. Operating System Configuration:
    - Install Apache
    - Send to the server config file `blog-vhost.conf` of Apache
    - Install `EPEL` and `Remi` repo 
    - Install `PHP-80`
3. WordPress Installation
    - Download Extract WordPress
    - Copy `blog-vhost.conf`
    - Restart `Apache`

# Screen of Working Wordpress
![Alt text](application.jpg)
