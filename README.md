
1.	Store all domain directories inside src folder
   
   i.	src/ - highest level of an app, contains common models, configs, and constants, etc.
   
  	ii.	src/main.py - root of the project, which inits the FastAPI app
   
2.	Each package has its own router, schemas, models, etc.
   
   i.	router.py - is a core of each module with all the endpoints
   
  	ii.	schemas.py - for pydantic models
   
  	iii.	models.py - for db models
   
  	iv.	service.py - module specific business logic
   
  	v.	dependencies.py - router dependencies
   
  	vi.	constants.py - module specific constants and error codes
   
  	vii.	config.py - e.g. env vars
   
 	viii.	utils.py - non-business logic functions, e.g. response normalization, data enrichment, etc.
  
   ix.	exceptions.py - module specific exceptions, e.g. PostNotFound, InvalidUserData
  	
3.	When package requires services or dependencies or constants from other packages - import them with an explicit module name


https://github.com/zhanymkanov/fastapi-best-practices/tree/master
