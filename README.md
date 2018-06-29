CouchDB Service for IIHS Application

CouchDB Service is integarted with Superlogin Service for Storing the data in Database.


## Deployment for Docker 
The CouchDB configurations are loaded from local.ini file.

## Configurations to be done in local.ini

- Admin Username and Password

      [admins]
      ;username=password                           // Set the Username and Passowrd in this Section
      
line no 101 and 102 in local.ini


- Enabling Cors in Couch DB


      [cors]
      origins = *                                  // Client URL or * for all origins
      credentials = true
      methods = GET, PUT, POST, HEAD, DELETE
      headers = accept, authorization, content-type, origin, referer, x-csrf-token

line no 103 and 107 in local.ini

## Deployment in Local

Download the Couchdb  from the [CouchDb Officical site](http://couchdb.apache.org/)

Install the CouchDB, after successfull installation 

Open the CouchDB Web Interface and configure the admin username and password

      http://localhost:portno/_utils
      (Eg: http://localhost:5984/_utils)
      
      
