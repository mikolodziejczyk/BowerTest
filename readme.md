# Bower fundamentals

E:\VisualStudio\Learn\BowerPractice\BowerTest

1. Installing Bower overview
 - installing github
 - installing bower
 - installing bower-installer
 - when?

2. Setup Bower in the project.
 - what file is requried
 - how to create it
 - should it be added to the source control?
 - how to prevent publishing it?

3. Installing registered packages with Bower, specifying the version
 - install jQuery, with the version exactly 1.9.1, registering this in the configuration file
 - how such an installation is represented in the configuration file
 - what means ~, why not to used it?
 - what means ^ at the beginning of the version? When it can be used?


4. Restoring dependencies on another machine: You have a predefined config file, at the bottom. 
Restore all the Bower packages to the local project.

  "dependencies": {
    "bootstrap": "^3.3.7",
    "jquery": "2.2.4",
    "jquery-migrate": "1.4.0"
  }

5. Copying dependencies to the destination folder with bower-installer
You want to copy key package files to the Dist folder. Every package should have its own subfolder 
with all the important files, e.g. Dist/jquery, Dist/bootstrap
 - what is the default way bower-installer works? What with minimized files?
 - how to configure bower-installer in the way that ensures all the important files are sent do dist?
 - In the case of jquery-migrate copy jquery-migrate.js and jquery-migrate.min.js

6. Configure the project to run bower-install with its settings from the previous point after each successful build.

7. Configure web publish in the way all Dist/ are published along with the application.


8. How to run bower-installer from grunt - e.g. to create a task in grunt that includes bower?


9. Intellisense files: jquery-1.8.2.intellisense.js, jquery.validate-vsdoc.js
 - what are intellisense.js and validate-vsdoc.js files?
 - where they are looked for?
 - what to do with the scripts originally in the scripts folder, how to preserve intellisense on js when possible?
 - what is _references.js file?
