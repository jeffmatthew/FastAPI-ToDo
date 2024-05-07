Endpoints:
Create Task
URL: /tasks
Method: POST
Description: Create a new task.
Request Body:
json
Copy code
{
    "title": "string",
    "completed": "boolean"
}
Response:
Status Code: 201 Created
Response Body:
json
Copy code
{
    "id": "integer",
    "title": "string",
    "completed": "boolean"
}
Get Task by ID
URL: /tasks/{task_id}
Method: GET
Description: Get task details by ID.
Response:
Status Code: 200 OK
Response Body:
json
Copy code
{
    "id": "integer",
    "title": "string",
    "completed": "boolean"
}
Get All Tasks
URL: /tasks
Method: GET
Description: Get details of all tasks.
Response:
Status Code: 200 OK
Response Body:
json
Copy code
[
    {
        "id": "integer",
        "title": "string",
        "completed": "boolean"
    },
    ...
]
Update Task
URL: /tasks/{task_id}
Method: PUT
Description: Update an existing task.
Request Body:
json
Copy code
{
    "title": "string",
    "completed": "boolean"
}
Response:
Status Code: 200 OK
Response Body:
json
Copy code
{
    "message": "string"
}
Delete Task by ID
URL: /tasks/{task_id}
Method: DELETE
Description: Delete a task by ID.
Response:
Status Code: 204 No Content
Delete All Tasks
URL: /tasks
Method: DELETE
Description: Delete all tasks.
Response:
Status Code: 204 No Content