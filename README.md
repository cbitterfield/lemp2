## LEMP: Linux | NGINX | MYSQP | PHP Docker Image

LEMP is a variation of the ubiquitous LAMP stack used for developing and deploying web applications. Traditionally, LAMP consists of Linux, Apache, MySQL, and PHP. Due to its modular nature, the components can easily be swapped out. With LEMP, Apache is replaced with the lightweight yet powerful Nginx.

![cbitterfield logo]<img src="https://github.com/cbitterfield/lemp/blob/master/cbitterfield_logo.jpg" alt="cbitterfield logo" width="250" >

logo by Anna Maria Paliasna Weaver (c) 2019

# This is a fully functional LEMP development environment with Secure Headers
This image is designed to be fully functional with data persitence.

## Capabilities:

* Start/Stop/Login script included for easy use
* Supports TLS self signed and real
* Allows for configuring database name, user and password via environment variables.
* Allows doe SSH/SFTP access by password and by key
* Includes a fully comprehensive example index.php to test LEMP functions
* Includes support for secure headers in TLS
* Fully documented scripts and docker file
* Fully configurable logging and debugging
* Fully configured with a seperate user and group for LEMP site (username = dev_site)
* Single mount point for host
* Uses docker volumes if not using host mount point

### Environment variables

**Variables:**
- LOG_LEVEL
- LOG_STDOUT
- MYSQL_DATABASE
- MYSQL_USER
- MYSQL_USER_PASS
- SITE_PASS
- SSH_PUBLIC
- TLS

## service script (lemp_service.sh)

usage lemp_service.sh [start|stop|status|show_docker|login|clear]

Script passes through any locally set variables.

login option runs interactive bash shell
clear option removes all containers in use

