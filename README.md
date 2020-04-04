# Reverse Engineering Code


! This app allows users to create an account, log into the account and sign back out securely.
 All user data is stored in a mysql database.





isAuthenticated.js 
{ restricts routes that user is not allowed to visit if not logged in. if user is logged in, it continues with request };





 config.json {
  connection configuration to connect to server };



passport.js {
  contains javascript logic that tells passport we want to log in with an email address and password };




index.js {
  connects to database and imports users log in data };

  user.js {
  requires "bcrypt" for password hashing. this makes our database secure even if compromised. Here we have JS that defines what is stored on our database };



Login.js{
Verifies if login exists and if it does, redirects to the members page}

Members.js{
This file just does get request to figure out which user is logged in
    and updates the HTML on the page}

Signup.js{
Getting references from signup form, if successful redirects to the members page}



Style.css{
Style for signup and login form}

.html{visual content in the browser}


api-routes.js { 
  contains routes for signing in, logging out and getting users specific data to be displayed client side };

 

 html-routes.js {
  routes that check whether user is signed in, whether user already has account etc and sends them tio the correct html page };




package.json {
contains all package info, node modules used, version info etc };

server.js {
requires packages, sets up PORT, creates express and middleware, creates routes and syncs database / logs message in terminal on successful connection to server };


