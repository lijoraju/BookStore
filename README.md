# BookStore Management APIs in Go Lang
Welcome to the BookStore Management API repository! This repository contains a set of APIs written in Go for managing a bookstore. Below are the details of the available APIs:

## Endpoints:

1. **GET /book/**
   - Retrieves details of all the books in the bookstore.

1. **POST /book/**
   - Creates a new book and adds it to the bookstore.
   - Request body should include:
      - name
      - author
      - publication

1. **GET /book/{bookId}**
   - Retrieves details of a specific book identified by the given `bookId`.

1. **PUT /book/{bookId}**
   - Updates details of a specific book identified by the given `bookId`.
   - Request body should include:
       - name
       - author
       - publication

1. **DELETE /book/{bookId}**
   - Deletes the book with the specified `bookId`.

## Database Configuration:

The application uses a MySQL server for database storage. To run the application locally, you need to update the database credentials in the `app.go` file located under the `config` folder.

## Running the Server Locally:

To run the server locally, follow these steps:

1. Navigate to the cmd/main directory:
   ```
   cd cmd/main
   ```
1. Build the application:
   ```
   go build
   ```
1. Run the application:
   ```
   go run main.go

The server will start running on port 9010, and you can access the APIs at the specified endpoints.

Feel free to explore, test, and integrate these APIs into your application. If you encounter any issues or have suggestions for improvement, please open an issue in this repository. Happy coding!
