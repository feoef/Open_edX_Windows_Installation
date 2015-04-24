2. Prerequisites
=============
This section describes the prerequisites for installing Open edX.

The Required Software Prerequisites
-----------------------------------

The Open edX platform has been implemented using a wide variety of software, including the python, ruby, and django programming languages, MySQL and mongodb database systems, the Nginx web server package, and the postfix email management system, to name a few.

To help ensure that the necessary software has been properly installed and configured to work together, several software installation and provisioning packages have been utilized.

To reduce the likelihood that the resulting edX development environment software will interfere with, or be disturbed by, other software already running on your computer, a virtual environment is used.
The virtual environment created allows you to install an additional operating system on your computer, where you can then install software and run the operating system and software alongside your original operating system, as if it were running on a separate computer.

In our case, we will use Microsoft Windows 7 Enterprise as the host operating system. 

Onto Windows 7 Enterprise, we will install a virtualization package and a few other software packages.

We will then execute a script provided by Open edX and its supporters that will create a virtual machine environment and install the rest of the edX platform software within that virtual machine environment.

You will need the following software:
 #. Windows 7 Enterprise 64-bit
 #. Virtual Box 4.3.16r95972
 #. Vagrant 1.5.4
 #. cURL for Windows 7.40.0
 
It would be helpful to go ahead and download these packages as a first step. Links to the packages are provided below.

| 
1. Microsoft Windows 7 Enterprise
---------------------------------

First, you will need the host operating system, Microsoft Windows 7 Enterprise, Service Pack 1.

You need the Enterprise (or Ultimate) version because that version comes with a systems service that the edX platform needs, called Client for Network File System (NFS).

Windows 7 Professional, and other versions of Windows 7, do not come with this NFS service.

You can buy a copy of Windows 7 Enterprise from Microsoft, a retail store, or online.

You can also download a 90 day evaluation copy of it from Microsoft here: 

- http://www.microsoft.com/en-us/evalcenter/evaluate-windows-7-enterprise

| 
2. Oracle VirtualBox
--------------------

Oracle VirtualBox is open source software you can use to install additional operating systems onto your computer.

VirtualBox will give you the ability to create a *virtual machine environment*, which is a separate operating system environment into which you can install software and store data.

You will need Oracle VirtualBox Version 4.3.16, and the companion extension pack for it.

NB: Earlier or more recent versions of this package need not necessarily work, so, be sure to get this version, in particular.

The homepage for Oracle VirtualBox: https://www.virtualbox.org/

You can find the versions you need for 64-bit Windows 7 here:

- http://download.virtualbox.org/virtualbox/4.3.16/VirtualBox-4.3.16-95972-Win.exe 
- http://download.virtualbox.org/virtualbox/4.3.16/Oracle_VM_VirtualBox_Extension_Pack-4.3.16-95972.vbox-extpack

| 

3. Vagrant
----------

Vagrant is open source software that will allow you to run scripts to more easily and reliably install and configure software.

A single Vagrant script will install the bulk of the operating environment for Open edX.

The Vagrant software version we will use is 1.5.4.

NB: Earlier or more recent versions of this package need not necessarily work, so, be sure to get this version, in particular.

The homepage for Vagrant: https://www.vagrantup.com/

You can find the Vagrant Version 1.5.4 that you need for 64-bit Windows here:

- https://dl.bintray.com/mitchellh/vagrant/vagrant_1.5.4.msi 

| 

4. cURL for Windows
-------------------

cURL for Windows is an open source command line tool and library for transferring data and downloading software using URL syntax.

This tool will be used to download the Vagrant script file that you will use to install the bulk of the edX environment.

The homepage for Confused by Code: http://www.confusedbycode.com/

You can find the curl version that you need for 64-bit Windows here:

- cURL for Windows web page - http://www.confusedbycode.com/curl/
- cURL for Windows direct download link - http://www.confusedbycode.com/curl/curl-7.40.0-win64.msi
