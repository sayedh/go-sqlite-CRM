# go-sqlite-CRM
Golang CRM APIs with SQLite. Create, read, update and delete data with Postman. 


## Technologies Used
* Golang
* SQLite
* Postman


## Dependencies
* Install Go - https://go.dev/doc/install
* Install SQLite - https://www.sqlite.org/download.html
* DB Browser for SQLite - https://sqlitebrowser.org/dl/ (not required)
* Install Postman - https://www.postman.com/downloads/


## Executing program
* Download the repository to your computer, go to project file, and run the code
```
git clone https://github.com/sayedh/go-sqlite-CRM
cd go-sqlite-CRM
go mod tidy
go run main.go
```

* Test APIs with Postman
  * Create a POST request to add data with http://localhost:3000/api/v1/lead
  ```
  {
    "ID": 2,
    "name": "Sayed Haque",
    "company": "Amazon",
    "email": "sayedh@amazon.com",
    "phone": 829923345345
  }
  ```
  * Create a GET request to get data by id with http://localhost:3000/api/v1/lead/1 (<-- 1 here is the ID, you can change to desired ID)
  * Create a GET request to get all data with http://localhost:3000/api/v1/lead
  * Create a DELETE request with http://localhost:3000/api/v1/lead/2 (<-- 2 here is the ID, you can change to desired ID)
