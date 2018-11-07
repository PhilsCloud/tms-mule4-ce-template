# A Mule 4 Community Edition Template

A Mule 4 community edition template, ideal boilerplate for your community edition project. The template includes routing, logging and error handling. Flows are split into config, error handling, API and logic mule configuration files to handle complex Mule applications.

## Global Configuration
The global configuration files handle the configurations for:
* HTTP Listener
* Global Error Handling
* APIKit Routing
* Configuration Properties

## Logging
The application comes with logging, taking the correlation ID, as well as other necessary details capturing the entry points into flows and the exit point of the API. 

## Error Handling
Global error handling has been implemented which creates the correct HTTP status codes while presenting an accurate error description to the client while logging additional information into the error log.
