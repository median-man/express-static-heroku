# Express-Static-Heroku

A demo of getting an Express app deployed as quickly as possible to follow the
mantra: "Deploy Early. Deploy Often."

## Overview

1. Setup git with .gitignore and make the first commit.
2. Initialize npm and install dependencies.
3. Setup the first route and home page.
4. Deploy!
5. Configure middleware to easily route to static files.
6. Re-deploy.

## Useful Express JS Functions

### `res.sendFile()`

Use to send a file back as the response to a request.

### `.use()`

Takes a function and runs that function every time a request is received. The callback is passed 3 arguments: `response, request, and next`.

### `app.use(express.urlencoded({ extended: true }));`

Allows the app to parse form data in a request and access it with `req.body`;

### `app.use(express.json());`

Allows the app to parse json data in a request and access it with `req.body`.

### `res.json()`

Send json data in the response going back to the client.
