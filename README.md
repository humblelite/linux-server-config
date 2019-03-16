# linux-server-config
Udacity server configuration project.

## I
The IP address and ssh port for the server project (178.128.64.7:2200).

## II
The website URL for the website is the IP address (178.128.64.7).

## III
Software install for this project includes: Apache2, Mod_wsgi, Python3, Python3-pip, Python-dev, and Postgresql.


#### Security
* Created  a new user with sudo privileges, 700 on .ssh directory and 644 on file.
* Generated and ssh key and placed the public key in the authorized_keys file.
* Next in sshd_config file I disabled the root login and password login. 
* Setup the UFW firewall by allowing ports 2200, 80, and 123 and enabling firewall.
* Then I changed the ssh port to 2200.

#### Apache2 Server
* Setup for the Apache2 server included creating a sites-available file for the application.
* Then using the Mod_wsgi documentation I setup the virtual host for the flask application. 
* Next I cloned my Github repo into the /var/www directory and created a WSGI file for the app.
* Created a virtual environment and install all of the packages for the app from requirements.txt file. 

#### Postgresql
* Opened database as postgres user and created database for the application.
* Then created a user for the database so that only the user has access to the database.

## IV
I used Digital ocean to setup up an ubuntu 16.04 server. Most of the third party resources I used where from Digital Oceans documentation and blog. I also used the  MOD_WSGI documentation and of course stack overflow when I ran into an issue.
