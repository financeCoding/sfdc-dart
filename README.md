PURPOSE/OBJECTIVE
=================

The purpose for this project is to illustrate how to create a Dart application that is powered by
force.com (salesforce). It describes how to access the force.com APIs, and leverage those within a 
Dart application. It uses Dart both on the server-side (to host the demo page) and the client (to 
program the interface). 

The demo application uses a tabbed interface to list all accounts and users related to a specific
salesforce.com instance.

For very detailed instructions on setting-up and running the project, see my blog entry 
at http://jeff-davis.blogspot.com/2013/04/using-forcecom-rest-apis-with-google.html

PREREQUISITES
=============

You must have Dart (version 0.4.3.5 or greater) installed locally (I would also recommend the Dart editor), and 
you must  have a force.com instance available to run the API calls against. Salesforce does provide a free 
developer version of force.com, so that should suffice.

SETUP
=====

1. After downloading the code, run "pub install" at the root directory level to install the required 
packages (as identified in the pubspec.yaml file). If the libraries identified in the yaml file have been
updated since this post, you may have to upgrade to the latest version of the Dart SDK.

2. When "pub install" correctly installs all of the dependencies, run "dart build.dart" from the root 
directory.

3. Update the constants.dart file to include your Salesforce credentials within the definition of LOGIN_CREDENTIALS.

4. Start the server component by running "dart bin/server.dart" (or "dart bin\server.dart" if on Windows).

5. Within the Dart IDE, right click on "sfdcdemo.html" and select 'Run in Dartium".




