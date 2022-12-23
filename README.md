This is a prototype for using nginx server as reverse proxy to achieve routing between different microfrontends

in order to run this project :
  -clone this repository
  -run the following command : docker-compose up
 what this will do : 
  this will build and deploy both application home and admin to your localhost and manage them using an orchestrator
  links matching with the route localhost/admin will map to the admin microfronted
  links matching with the route localhost/home will map to the home microfronted
 
 This is merely a proof of concept
 
