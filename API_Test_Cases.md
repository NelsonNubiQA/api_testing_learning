TC001: Verify Existing User Information Can Be Retrieved
Method: GET
Endpoint:
/api/users/2
Expected Results:
Status code 200 is returned.
The response contains user ID 4.
The user's email is returned.
The user's first name is returned.
The user's last name is returned.


TC002: Verify New User Record Can Be Created
Method:POST
 
Request Body
{
  "First Name": "George"
   "Last Name": "Brown"
    "Job": "SQA"
}
Endpoint 
/api/users
Expected Results:
Status code 201 is returned.
A new user record is created successfully.
A unique user ID is generated.
The response contains the submitted user details.
A creation timestamp is returned.

TC003: Verify Existing User Information Can Be Updated
Method: PUT
Endpoint 
/api/users/4
Request Body
{
  "job": "AI Engineer"
}
Expected Results:
Status code 200 is returned.
The user's job is updated successfully.
The response contains the updated job value.
An updated timestamp is returned.


TC004: Verify Existing User Can Be Deleted
Method: DELETE
Endpoint
/api/user/4
Expected Result
	1. Status code 204 is returned.
	2. The user is deleted successfully.
	3. No response body is returned. 
