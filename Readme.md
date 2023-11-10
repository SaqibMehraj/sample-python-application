# Readme for Simple Web Server

This project demonstrates how to create a simple web server using Python's built-in `http.server` module.

## Dependencies

1.This project requires Python 3.5 or higher.
2.Docker engine


## How to Run

To run the server, follow these steps:

1. Clone this repository in your server
2. Build the image using ```docker build -t sample-application .```
3. Execute the image using ```docker run -p 8000:8000 sample-application```
4. The server will start and you will see a message saying `Server running at localhost:8000...`.

## Accessing the Web Server

Once the server is running, you can access it by opening a web browser and navigating to `http://localhost:8000/`.

## Code Overview

The code consists of the following:

- `SimpleHTTPRequestHandler`: This class is used to handle HTTP requests and responses. In this example, the `do_GET` method is overridden to return a "Hello, World!" message.

- `run`: This function sets up the server to listen on port 8000. When a request is received, it is handled by an instance of the `SimpleHTTPRequestHandler` class.

To learn more about how the `http.server` module works, you can refer to the official Python documentation: https://docs.python.org/3/library/http.server.html
