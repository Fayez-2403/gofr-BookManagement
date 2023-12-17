💡 # GoFr Bookstore
The GoFr Bookstore is a comprehensive book management system built on the GoFr framework, incorporating seamless integration with Redis and MySQL databases. This README provides step-by-step instructions for setting up and running the application.

# To get started with GoFr use the following command:

```bash
go get gofr.dev
```

The latest version of go in your system should be installed.

## API Requests made using postman

## 1. GET ALL Request

- Get all the Books
  ![GET ALL](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/1e80e07a-ba08-4ef6-b9d9-629e93392679)

## 2.CREATE Request

- Add books to table

![Create](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/c8b1f0f9-59dd-4937-85f5-435cf94ffcde)

## 3.GET BY ID Request

- Fetch book by BOOK ID

![GET BY ID](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/69dc9bd4-6244-445e-88f2-3d29721eebb2)


## 4.UPDATE Request

- UPDATE the book's Author

  ![UPDATE](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/bfc49aee-e4a0-48e9-9f23-3e0b4c12a60f)

## 5.🗑️ DELETE Request

- Deletes an existing book record

  ![DELETE](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/9a5373a6-efd8-4dff-9048-47406344811d)

# UML Diagrams

- Project Structure

  ![project structure](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/15e61d6e-039e-40b6-ac73-ae35c221394e)

- ROUTES

  ![routes](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/3e743225-2b00-46e0-9a0d-f6010c85c605)

# Database 🛢️

The project utilizes a MySQL database to store information about book. The MySQL database is set up as a POSTMAN container for easy deployment and management.

## Database Schema 🗃️

- Table: `books`
  - Columns: `id` INT AUTO_INCREMENT PRIMARY KEY,
    `name ` VARCHAR(255) NOT NULL,
    `author ` VARCHAR(255),
    `publication ` VARCHAR(255)
    ![db schema](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/cb0859fd-ea68-4a69-8c53-e81c305359f8)

## Database Setup 🐳

- POSTMAN Container
 ![database setup](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/6da226be-fde9-4110-ad86-fa4aebda8508)

- To run the MySQL database locally as a postman container, use the following command:

```bash
mysql xmysql -h localhost u-Fayez-2403 -p Fayez@1724 -d bookstore
3306:3306 -d mysql:8.0.30
```

- After this create a new connection in MYSQL workbench and make a projects table with the above defined schema to successfully setup the database.

# ⚡️ RUN

- Now simply run the following command in your terminal to run the application:

```bash
go run cmd/main.go
```

# cmd/main.go

![main go](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/8c7e5ca0-5bf8-4c4a-a3d5-feb586a83b25)

# pkg/config/app.go

![app go](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/781d7139-9f1e-4f2d-88df-e71f4c55afdf)

# pkg/controllers/book-controller.go

![book-controller-go](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/e8beeb3c-4b62-475b-b993-505e44d4631a)

# pkg/models/book.go

![book go](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/e763de76-bf62-4647-9d93-8e697072438e)

# pkg/routes/bookstore-routes.go

![bookstore-routes go](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/a240b449-12c5-4182-ac01-d4616c151e7c)

# pkg/utils/utils.go

![utils go](https://github.com/Fayez-2403/gofr-BookManagement/assets/79997853/7c35d91b-907a-47e9-8b32-5a783778f83a)
