# Learning Go: A Simple Web Server Example

Welcome to the "Learning Go" project! This repository contains a basic example of a web server written in Go. As I am new to Go (Golang) and wanted to see a practical example of how to build and run a web server in Go.

## Project Overview 🔎

This tutorial project of demonstrates a simple web server built using the Go programming language. The server includes:

- A file server to serve static files from the `./static` directory.
- A form handler to process and display form submissions.
- A basic hello world handler to respond to GET requests.

## Getting Started 🌟

### Prerequisites 📃

Make sure you have Go installed on your machine. If not, you can download and install it from the [official Go website](https://golang.org/dl/).

### Setup ⚙

**Clone the repository:**

```
git clone https://github.com/natejonesiii/goserver.git
cd goserver
go build
./goserver
```

You should see the message Starting server on port 8080.

#### Open your web browser and visit: 🌐

```
http://localhost:8080/ to access the static files.
http://localhost:8080/form to test the form handler. (Submit form data with fields named name and address).
http://localhost:8080/hello to see the "Hello World from Go!" message.
```

### Code Explanation 🤯

- formHandler: This handler processes POST requests sent to the /form endpoint. It parses form values and displays the submitted name and address.

- helloHandler: This handler responds with a "Hello World from Go!" message to GET requests sent to the /hello endpoint. It also handles 404 errors for invalid paths and methods.

- main: The main function sets up the HTTP server. It uses http.FileServer to serve static files from the ./static directory, and it registers the form and hello handlers.

### Contributing 👥

Feel free to fork the repository and make improvements. If you find any issues or have suggestions, please open an issue or submit a pull request.
