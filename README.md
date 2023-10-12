# API CRUD 
This api lets you insert, delete, view, and update names on the database.


## API Description
This api is created to directly manipulate the contents of a database using the four (4) api endpoints. But in order to run, you must first create a database named 'demo', with a table named 'names', and columns called id (PK, AI), lname, and fname. 

But inorder to use this api, you must first install postman which can be downloaded in the link below:
https://www.postman.com/downloads/

 
## API Endpoints
The API is composed of four (4) endpoints.

Endpoint 1: 'postName'
This endpoint accepts the lname and fname parameters and inserts/stores it in the database.

Endpoint 2: 'printName'
This endpoint does not necessarily need a Request Payload but immediately returns a Response Payload that prints the database contents in JSON format.

Endpoint 3: 'updateName'
This endpoint updates the current content of the database by accepting an 'id', 'lname', and 'fname' parameters. It uses the 'id' parameter as the basis as to which record is to be updated.

Endpoint 4: 'deleteName'
This endpoint accepts the 'id' parameter and deletes a record on the database based on the 'id' number.


## Request Payload

Endpoint 1: 'postName'
{
  "lname":"Tamad",
   "fname":"Juan"
}

Endpoint 2: 'printName'
This endpoint does not need a Request Payload as it automatically prints the Response Payload which is the contents of the database in JSON format.

Endpoint 3: 'updateName'
{
  "id":1,
  "lname":"Dela Cruz",
   "fname":"Juan"
}
note: the 'id' is necessary as it is the basis as to which record is to be updated.

Endpoint 4: 'deleteName'
{
  "id":1
}
note: 'id' is the only necessary parameter in deleting records in the database.
 

## Response Payload

Endpoint 1: 'postName'
{
         "status":"success","data":null
}

Endpoint 2: 'printName'
{
         "status":"success","data":["lname":"hortizuela","fname":"manny","lname":"licayan","fname":"arnold"]
}

Endpoint 3: 'updateName'
{
         "status":"success","data":null
}

Enpoint 4: 'deleteName'
{
         "status":"success","data":null
}


## Usage
Step 1: Open your XAMPP or SQLyog
Step 2: Create the database 'demo' and the table 'names' with columns 'id', 'lname', and 'fname'. 'id' being the primary key and auto increment
Step 3: Store the api folder in the folder C:// >> xampp >> htdocs
Step 4: Install and open Postman
Step 5: Set HTTP Method whether it is GET or POST
Step 6: Enter the url 
For endpoint 'postName':  localhost/api/public/postName
For endpoint 'printName':  localhost/api/public/printName
For endpoint 'updateName':  localhost/api/public/updateName
For endpoint 'deleteName':  localhost/api/public/deleteName
Step 6: Open the 'Body' tab and enter the JSON Request Payload

 
## License
No license used.


## Contributors
Mr. Manny R. Hortizuela
 
## Contact
Email: rolandgracias26@gmail.com
