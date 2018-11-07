# A Mule 4 Community Edition Template

A Mule 4 community edition template, ideal boilerplate for your community edition project. The template includes routing, logging and error handling. Flows are split into config, error handling, API and logic files to handle complex Mule applications.

## Global Configuration
The global configuration file handles the configurations for:
* HTTP Listener
* Global Error Handling
* APIKit Routing
* Configuration Properties

## Logging
The application comes with custom logging, a custom logging component which I have extended to add additional information and make easier to configure your own. In order for this project to compile you will need to download the custom logging component (https://github.com/tom-murray/custom-logging), and run the command 'mvn clean install' in the root of the component folder which will install the component in to your local maven repository allowing you to run this template.

## Error Handling
Global error handling has been implemented which creates the correct HTTP status codes while presenting an accurate error description to the client while logging additional information into the error log.

## Maven Gitflow Helper plugin
The POM file contains some elements of the Gitflow Maven Helper Plugin, in order to active the plugin you will need to make some configuration changes and ensure you have a Nexus repository up and running along with the likes of Jenkins or Bamboo. Further details on the plugin can be found here: https://github.com/egineering-llc/gitflow-helper-maven-plugin
