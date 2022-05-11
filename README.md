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
* Download the repository to your computer and go to project folder
```
git clone https://github.com/sayedh/go-MySQL-Bookstore
cd go-MySQL-Bookstore
code .
```


* Update app.go file with your MySQL identity
  * (username):(password)@/(schema) EX: root:mysql@/simplerest
 


* Run the code
```
go mod tidy
go run main.go
```
  
## Test APIs with Postman
 * Create a POST request to add data with localhost:9010/book/
 ```
{
    "Name":"The startup way",
    "Author":"Eric Ries",
    "Publication":"Penguin"
}
 ```
 * Create a GET request to get data by ID with localhost:9010/book/2 (<-- 2 is the ID of the data)
 
 * Create a PUT request to update book data with localhost:9010/book/2
   * (2 is the ID of the data, can be changed to desired data that needs to be updated)
 ```
{
    "ID": 2,
    "name": "The startup way",
    "author": "Eric Ries",
    "publication": "Orion"
}
 ```
 * Create a GET request to get all data localhost:9010/book
 * Create a DELETE request with localhost:9010/book/3
   * (3 is the ID of the data, can be changed to desired data that needs to be deleted)
