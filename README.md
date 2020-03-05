## To use it
Git clone the folder and check out the .env.sample and create your own .env file.

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
This is where you can log in. However, you may need to register a new account if you haven't got any.

<img src="/images/login.PNG" align="left" hspace="20" /> <img src="/images/signup.PNG" align="left" hspace="20" /> 
 
 The home page with only logout button(currently).
 <img src="/images/home.PNG" />
 
 The grid page showing the data by table.
 <img src="/images/grid.PNG" />
 
 And you can search by the offence or filter by optional params.
 <img src="/images/gridWithFilter.PNG" />
 
 The graph page.
 <img src="/images/graph.PNG" />
 
 The map page.
 <img src="/images/map.PNG" />
