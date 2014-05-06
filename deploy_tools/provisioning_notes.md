Provisioning a new site
=======================

## Required packages:

* nginx
* Python 3
* Git
* pip
* virtualenv

eg, on Ubuntu:

	sudo apt-get install nginx git python3 python3-pip
	sudo pip3 install virtualenv

## Nginx Virtual Host config

* see nginx.template.conf
* replace SITENAME with, eg, staging.my-domain.com

## Upstart Job

* see gunicorn-upstart.template.conf
* replace SITENAME with, eg, staging.my-domain.com

## Folder structuter:
Assume we have a user account at /home/username

/home/username
/home/username/sites
/home/username/sites/SITENAME
/home/username/sites/SITENAME/database
/home/username/sites/SITENAME/source
/home/username/sites/SITENAME/static
/home/username/sites/SITENAME/virtualenv
