# Practice 

In this exercise, you will create API endpoints to insert a new category and retrieve a furniture record based on categoryid. Follow the instructions below: 

## Instructions

1. **Clone the repository**: Clone this repository to your local machine.

   ```shell
   git clone https://github.com/your-username/your-repository-name.git
   ```

2. **Navigate to the repository**: Change to the repository's directory.

   ```shell
   cd your-repository-name
   ```

3. **Install dependencies**: Install the necessary dependencies by running the following command.

   ```shell
   npm install
   ```

4. **Implement your Express.js application**: Create your Express.js application with the required endpoints and/or functionality based on the following specifications.

      **Basic Part 1**
      POST request to create a new category      

      1.Method: POST
      Endpoint: http://localhost:3000/category
      Body (JSON): 

      {
       "name": "Cupboards",
        "description": "Good and reliable storage spaces"
      }

      Expected Behavior:
      If the insertion is successful:
      Create a new category.
      Return a success message if the operation is successful.
      Status Code: 201 Created

      Sample Response:
      {
      "message": "New Category created successfully."
      } 

      If the insertion fails:
      Return an appropriate error message with a status code of 500.

     **Basic Part 2**
      GET request to retrieve a furniture from a particular category:

      Method: GET
      Endpoint: http://localhost:3000/category/:categoryId/furniture
      Params:
      categoryId: The ID of the category to retrieve.
      Body: Leave it empty

      Sample Response:
      {
      "fid": 1,
      "name": "Brown Leather Sofa",
      "description": "Stylish and suitable for all homes",
      "price": "500",
      "quantity": 20,
      "catid": "1",
      "catName": "Sofa"
    
      }

    If error occurs
    Return an appropriate error message with a status code of 500.

5. **Submit your solution**:
   Once you finish testing your application, you can submit your solution for grading.

   Note: Make sure your Express.js application follows the specified endpoint URLs and handles requests and responses correctly according to the given instructions.
