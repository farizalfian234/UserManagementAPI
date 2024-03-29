Design Choices:

- Model Design:
  I chose a simple User model with properties for UserId, FirstName, LastName, and
  Email. These properties are marked with data annotations for validation purposes.

- Controller Structure:
  The UserController class is structured to follow RESTful conventions, with separate
  methods for each CRUD operation.
  
- In-Memory Data Storage:
  For simplicity, I used an in-memory list to store user data. In a production environment,
  you would typically use a database like SQL Server.
  
- Input Validation:
  I implemented basic input validation using data annotations in the model class and
  checked ModelState.IsValid in controller methods to ensure data integrity.
  
- Error Handling:
  Error handling is implemented using standard HTTP status codes. For example,
  returning 404 Not Found when a user is not found.
  
- Middleware Configuration:
  The API is configured with minimal middleware, including routing and JSON
  serialization.


Instructions to Run and Test the API:

1. Clone the Repository: Clone the repository containing the ASP.NET Core API project to
your local machine.
2. Open in Visual Studio: Open the solution file (.sln) in Visual Studio 2022.
3. Build the Solution: Build the solution to restore NuGet packages and compile the project.
4. Run the API: Start the API by pressing F5 or using the Debug menu.
5. Test the API:
  a. You can test the API using tools like Postman, curl, or any HTTP client.
  b. Use the following endpoints to perform CRUD operations:
    i. Create a new user: Send a POST request to /api/user with JSON data
    representing the user.
    ii. Retrieve all users: Send a GET request to /api/user.
    iii. Retrieve a single user by ID: Send a GET request to /api/user/{userId}.
    iv. Update a user: Send a PUT request to /api/user/{userId} with JSON data
    representing the updated user.
    v. Delete a user: Send a DELETE request to /api/user/{userId}.
   
By following these instructions, you should be able to run and test the API locally on your
machine. If you encounter any issues or have any questions, feel free to ask for assistance.
