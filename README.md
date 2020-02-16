## API Routes 

* GET request without JWT verification
  * /offences => returns an array of offences recorded.
  * /areas => returns array of Local Government Areas.
  * /area/:id => returns the location of specific area.
  * /ages => returns an array of age categories. 
  * /genders => returns an array of gender categories. 
  * /years => returns an array of years recorded. 
  
* GET with JWT verification
  * /search?offence=xxx&param1=xxxx&param2=xxxx => The primary search route, with required offence and optional filter parameters, which again must be url encoded. (Requires authentication). Params must be one of: area, age, gender, year.
  
* POST 
  * /register => Register using email and password 
  * /login => Logging into your account using the details provided. This allows access to authenticated routes via a JSON Web Token. 
  
