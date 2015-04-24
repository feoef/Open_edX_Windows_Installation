11. Install Custom Theming
==========================
It is possible to customize the look-and-feel of your instance of Open edX, though it might not be as simple and straightforward as some might like.

The team at edX.org says that they plan to provide a more straightforward means of doing so at some point in the future.

Meanwhile, the theme known as the "Stanford-Online edX Theme" is available, and is said to provide some facility whereby one can more easily customize the learning management system (LMS) of Open edX. 

   .. image:: https://cloud.githubusercontent.com/assets/8691899/7189110/8386388a-e44a-11e4-99a0-59b7b8373943.jpg


The content management system (CMS) Studio look-and-feel will not affected by this customization.

The Process
^^^^^^^^^^^
1. Log into the Ubuntu instance, using the vagrant User ID (the ID and password are each vagrant).

2. Modify the lms.env.json file that can be found in the /edx/app/edxapp directory.
   You can do so with the character-based editor nano, using the following command:
     
   sudo nano /edx/app/edxapp/lms.env.json

3. In the json file, change "USE_CUSTOM_THEME": false to "USE_CUSTOM_THEME": true

4. Also change "THEME_NAME": “" to "THEME_NAME": "default"

5. Save the file, using CTRL O.

6. Close the file using CTRL X.

7. Become the edxapp user, by executing the following line:
   
   sudo su edxapp -s /bin/bash
   
8. Execute the following lines:
   
   cd ~

   source edxapp_env

9. Create a directory for the theme and then download the Stanford theme from github into that directory:
   
   mkdir themes

   cd themes
   
   get clone https://github.com/Stanford-Online/edx-theme.git default

10. Recompile the edX assets:

    cd /edx/app/edxapp/edx-platform
   
    paver update_assets lms --settings-aws

Upon successful completing of the above steps, you will see the Stanford Theme upon restarting the web server.

