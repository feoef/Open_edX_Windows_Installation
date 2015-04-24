# Open_edX_Windows_Installation
Installing Open edX on Windows 7 

Introduction
============

Open edX is the software that powers edX-related online learning websites, such as edX, HarvardX, and MITX, among many others.

Open edX includes a:
 
- Learning management system (LMS) which allows users to register for and take courses.
- Content management system (CMS) called Studio which allows authors to create content.

The Open edX environment has been built on open source software. Open source software is software that has been licensed to be used by the general public for free.

edX software utilizes more than twenty four open source software languages, utilities, and technologies.

The operating system on which edX is based is Ubuntu, an open source variant of Linux. The primary base programming language used to create edX is python.

Open edX provides scripts and documentation that can be used to install the Open edX environment.

|

The Goal
--------

The ultimate goal of this documentation is to help you install a working copy of Open edX on a single computer, whereby a content developer could immediately use it to develop Open edX courses.

These instructions will describe the steps suggested to install a copy of the Aspen.1 production release of Open edX on a single Windows 7 Enterprise based personal computer.

|

The Overall Process
-------------------

The overall installation process will involve the following major steps:
 
1. Install Windows 7 Enterprise Service Pack 1 and enable the Network File System (NFS) service.
 
2. Download additional required software. 
 
3. Install the Oracle Virtual Box virtualization package.
 
4. Install the Vagrant provisioning and installation package.
 
5. Install the curl command line-based file transfer program.
 
6. Use Vagrant to download and install the Open edX environment.
 
7. Install several additional useful software utilities.
 
8. Install and configure the mail system software.
 
9. Install and configure the Open edX-related Stanford Custom Theme.
 
|

The Result
----------

After successfully installing the Open edX environment, you will have the ability to:
 
 - Login to the Learning Management System (LMS). 
 - Login to Studio, the Content Management System (CMS).
 - Register as a new user (student or staff member).
 - Register to take a course.
 - Create new courses and content as a content provider and publisher.
 - Access the edX content from a browser running on your host operating system.
 

These steps will not necessarily make the courses available to anyone else, over the internet or otherwise.

The courses developed using this system could, however, be exported and then imported into a system that is accessible from the internet.


|

Initial Contributors
--------------------
- Derrick Lewis
- Nilesh Londhe
- Suart O'Day

