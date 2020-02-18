## SQL Setup
The server here uses MySQL for database. You will find the downloads here: https://dev.mysql.com/downloads/mysql/ and you should choose one appropriate to your OS. Accept the defaults and install as a service if you are using windows.

With mysqldump.sql file in database directory, you should be able to load the script file and run the script. Check this video out if you want to know how to do it: https://www.youtube.com/watch?v=POcHaIwmAhw.

## API Routes 
* GET request without JWT verification
  * /offences => returns an array of offences recorded.
  * /areas => returns array of Local Government Areas.
  * /area/:id => returns the location of specific area.
  * /ages => returns an array of age categories. 
  * /genders => returns an array of gender categories. 
  * /years => returns an array of years recorded. 
  
* GET with JWT verification
  * /search?offence=xxx&param1=xxxx&param2=xxxx => The primary search route, with required offence and optional filter parameters. Params must be one of: area, age, gender, year.
  
* POST 
  * /register => Register using email and password 
  * /login => Logging into your account using the details provided. This allows access to authenticated routes via a JSON Web Token. 
  
  
## Front-end pages
Coming soon!
  
  
