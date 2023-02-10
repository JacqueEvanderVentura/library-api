# Book API

A RESTful API for books.

## Getting started

### `yarn`

Installs the required dependencies to run the project.

### `yarn dev`

Runs the server in development mode.
Visible in MongoDBCompass with the mongodb://localhost:27017 URI.

The server will automatically reload on file save.

## Routes

### `POST /books`

This route creates two books with 5 pages each.

### `GET /books`

This route retrieves a list of all books.

### `GET /book/:bookId/page/:page/:type`

This route retrieves a specific page from a book.

#### Parameters

- `bookId`: The ID of the book, generated by the database.
- `page`: The number of the page to retrieve (starting from 1).
- `type`: The format of the page to retrieve, either `html` or `text`.


### Examples

#### Get all books

`GET /books`


#### Seed books

`POST /books`


#### Get a specific page in HTML format

`GET /book/123/page/2/html`


#### Get a specific page in TXT format

`GET /book/456/page/3/text`


## Time used to complete test

Around 2 hours in total, separated in different chunks of Feb 8 2023 and Feb 9 2023.
