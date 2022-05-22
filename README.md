# Archery
The Archery webserver is desigined to be a way for archery enthusiasts to share or view any event related to Archery
These events are called connections and users can create/delete/view/update/rsvp connections depending on their authorization for a particular function

Archery is coded with the node express web framework on javascript
The software of this application has multiple features that you would find in a live secure webserver including

-serverside input validation and output encoding with the express validator package to prevent xss or buffer overflow attacks

-cliet side input validation on the ejs view pages

-bcrypt to hash passwords

-limit authentication request using express rate limit package to prevent bruteforce attacks

-mvc software pattern

-Mongoose to integrate a MongoDB database

-EJS pages to present the view to the browser.

-modularized routes to forward the request to the appropriate controller function.

-moularized controller to control the flow of the application.

-app reinforces secure aauthorization rules mainly through validators built and called by the routes before being sent to controllers

-error handling

-short lived persistent sessions stored in db


Startup
1. Install nodejs if not already installed
   https://nodejs.org/en/
  
2. Install mongodb as a service if not already
   https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-windows/
   
3. The application connects to the default local mongodb which is at port 27017
   Attached in this repository is the startupDB file that contains some dummy data to populate the website and demonstrate its functionality that you can optionally      choose to run on a mongodb shell or you can startup the application without it
   Mongo shell Installation Instrictuins: 
   https://www.mongodb.com/docs/mongodb-shell/install/#std-label-mdb-shell-install
   
4. Navigate to the unzipped Archery directory on your powershell and run:
   node app
   
5. http://localhost:3000/


