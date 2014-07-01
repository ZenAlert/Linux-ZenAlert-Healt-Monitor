Linux-Healt-Monitor
===================


## Overview

"Linux Health Monitor" uses ZenAlert Cloud Platform to alert you in case of disk space low, absence of electricity or connectivity of the computer / server / device.

## Requirements

* Unix-like System
* cUrl 
* ZenAlert free account

## Installation

Start with installing curl:
	
	* sudo apt-get install curl (in debian/ubuntu)
	* sudo yum install curl (in redhat/centos)


* Save healtmonitor.sh on your disk
* Make script executable: chmod +x healtmonitor.sh
* Use crontab for execute the script every five minute

edit crontab configuration file:

	crontab -e
    

and append this line at end of crontab configuration file:
	
	*/5 * * * * /mypath/healtmonitor.sh
	
save and exit
