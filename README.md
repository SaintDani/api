"# api"

# API Name

JSON POST


 


## API
Description

This API endpoint allows clients to send data to a server for tasks such as creating new entries or modifying existing ones. The data is sent in JSON format in the request body, simplifying the data exchange. The server replies with an HTTP status code and a JSON response that carries pertinent details. This API can serve multiple purposes, ranging from user registration to data modifications or even initiating custom operations, and it incorporates security measures to ensure safe access. 




## API
Endpoints


Describe the
available endpoints, their functions, and the required parameters.

http://127.0.0.1/api/public/postName
- function: insert data into the database
- parameteres: fname , lname

http://127.0.0.1/api/public/postUpdate
- function: update the existing data in the database
- parameters: id , lname, fname

http://127.0.0.1/api/public/postPrint
- function: It will display the data inside the database
- parameters: none

http://127.0.0.1/api/public/postDelete
- function: It will delete data from the database
- parameters: id
 


## Request
Payload

JSON Payload postName:

Request payload:
- {
  "lname":"hortizuela",
   "fname":"manny"
}

 JSON Payload printName:
 
Request payload:

JSON Payload updateName:

Request payload:
- {
  "id":1,
  "lname":"wick",
   "fname":"john"
}

JSON Payload deleteName:

Request payload:
- {
  "id":1
}

## Response
JSON Payload postName:

- Response payload:
- {
         "status":"success","data":null
}

JSON Payload printName:

- Response payload:
- {
         "status":"success","data":["lname":"hortizuela","fname":"manny","lname":"licayan","fname":"arnold"]
}


JSON Payload updateName:

- Response payload:
- {
         "status":"success","data":null
}


JSON Payload deleteName:

- Response payload:
- {
         "status":"success","data":null
}



 


## Usage
Provide code
examples or instructions on how to use your API.

To use the provided API endpoints for inserting, updating, printing, and deleting data from the database using Postman, follow these steps:

1. Open Postman:

Make sure you have Postman installed and running.

2. Send a POST Request to Insert Data:

For inserting data into the database using the /api/public/postName endpoint:

Set the HTTP method to POST.
Enter the URL: http://127.0.0.1/api/public/postName.
In the request body, provide the parameters fname and lname with the values you want to insert into the database.
Click the "Send" button to send the request.


3. Send a POST Request to Update Data:

For updating existing data in the database using the /api/public/postUpdate endpoint:

Set the HTTP method to POST.
Enter the URL: http://127.0.0.1/api/public/postUpdate.
In the request body, provide the parameters id, fname, and lname with the values you want to update in the database.
Click the "Send" button to send the request.


4. Send a POST Request to Print Data:

For displaying data from the database using the /api/public/postPrint endpoint:

Set the HTTP method to POST.
Enter the URL: http://127.0.0.1/api/public/postPrint.
Leave the request body empty since it doesn't require any parameters.
Click the "Send" button to send the request.


5. Send a POST Request to Delete Data:

For deleting data from the database using the /api/public/postDelete endpoint:

Set the HTTP method to POST.
Enter the URL: http://127.0.0.1/api/public/postDelete.
In the request body, provide the parameter id with the ID of the data you want to delete.


Click the "Send" button to send the request.

 


## License

No License 


## Contributors

Sir Manny Hortizuela
provided:

- some codes
- database structure
- payloads
- etc.


## Contact
Include contact
information for inquiries or support.

Danica R. Gatchallan 
- danica.gatchallan@student.dmmmsu.edu.ph
- 09635547298
- 09703936709
