# Build-a-REST-API
This repository contains the code and instructions to build a RESTful API using Node.js and Express. The API will serve as a foundation for creating, reading, updating, and deleting resources.

# API Endpoints
1. Get all resources
Endpoint: GET /resources
Description: Retrieves all resources.
Example Response:
json
Copy code
[
  {
    "id": 1,
    "name": "Resource 1",
    "description": "Description of Resource 1"
  },
  {
    "id": 2,
    "name": "Resource 2",
    "description": "Description of Resource 2"
  }
]
2. Get a specific resource
Endpoint: GET /resources/:id
Description: Retrieves a specific resource by its ID.
Example Response:
json
Copy code
{
  "id": 1,
  "name": "Resource 1",
  "description": "Description of Resource 1"
}
3. Create a new resource
Endpoint: POST /resources
Description: Creates a new resource.
Request Body:
json
Copy code
{
  "name": "New Resource",
  "description": "Description of the New Resource"
}
Example Response:
json
Copy code
{
  "id": 3,
  "name": "New Resource",
  "description": "Description of the New Resource"
}
4. Update a resource
Endpoint: PUT /resources/:id
Description: Updates an existing resource.
Request Body:
json
Copy code
{
  "name": "Updated Resource",
  "description": "Updated description of the Resource"
}
Example Response:
json
Copy code
{
  "id": 1,
  "name": "Updated Resource",
  "description": "Updated description of the Resource"
}
5. Delete a resource
Endpoint: DELETE /resources/:id
Description: Deletes a resource by its ID.
Example Response:
json
Copy code
{
  "message": "Resource with ID 1 deleted successfully"
}
Technologies Used
Node.js
Express
