Golang HRMS APIs with MongoDB. Create, read, update and delete HR employee with Postman. 

## Technologies Used
* Golang
* MySQL
* Postman


## Dependencies
* Install Go - https://go.dev/doc/install
* Install MySQL - https://dev.mysql.com/downloads/installer/
* Install Postman - https://www.postman.com/downloads/


## Executing program
* Download the repository to your computer, go to project file, and run the code
```
git clone https://github.com/sayedh/go-MySQL-Bookstore
cd go-MySQL-Bookstore
cd cmd/main/
go mod tidy
go run main.go
```
* Update app.go file with your MySQL identity
  * <username>:<password>@/<schema> EX: root:mysql@/simplerest
  
* Download the repository to your computer, go to project file, and run the code

  
* Test APIs with Postman
  * Create a POST request to add data with http://localhost:3000/employee
  ```
  {
    "name":"Sayed Haque",
    "salary":1234567,
    "age":29
  }
  ```
  * Create a GET request to get all data with http://localhost:3000/employee
  * Create a PUT request to update employee data with http://localhost:3000/employee/627af1fa0903ad2cbc8f6c21 (<-- the 627xxxxxxx is the ID of the data, can be changed to desired data that needs to be updated)
  ```
  {
    "name":"Sayed Haque",
    "salary":87654321,
    "age":29
  }
  ```
  * Create a DELETE request with http://localhost:3000/employee/627af1fa0903ad2cbc8f6c21 (<-- the 627xxxxxxx is the ID of the data, can be changed to desired data that needs to be deleted)
