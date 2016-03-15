FDM Tracker Development Environment
====================

Apache Tomcat Server 8.0.32 running on Ubuntu 14.04.4 LTS (Trusty Tahr)


Installation
------------

Make sure you have [Virtual Box](https://www.virtualbox.org/wiki/Downloads) installed on your machine.

Install [Vagrant](https://www.vagrantup.com/downloads.html) to setup and configure the Development Environment.

Download a zip of this repository and unpack the contents. Enter into that folder in the command line and type in:

    vagrant up

Usage
-----

To enter into the Ubuntu Virtual Machine on a Mac you simply type in:

    vagrant ssh

To enter into the Ubuntu Virtual Machine on Windows you will have to use PuTTy.

    vagrant ssh

Typing in the above command will give you the Host and Port information.

The Username and Password are both **vagrant**.

It Just Works!
------------

The Tomcat Server is installed and up and running.

To verify that the service is running type in:

    initctl status tomcat

To see the start up page in your browser type in:

    ifconfig

The output next to eth1 - inet addr: xxx.xx.x.xxx is the server ip address.

In your web browser type in:

	xxx.xx.x.xxx:8080

Unlocked Features
-------

Synced Folders and Vagrant Share have both been disabled by default.

In the Vagrantfile uncomment out the bottom of the file to enable.

To Stop the FDM Tracker Development Environment
-------

Simply type in:

    vagrant halt

To Delete the FDM Tracker Development Environment
-------

Simply type in:

    vagrant destroy
