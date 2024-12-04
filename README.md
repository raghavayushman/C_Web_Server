
# Web Server in C

## Overview
This project is a simple, lightweight web server written in C that demonstrates the fundamentals of handling HTTP requests and serving content. It is designed to process incoming client requests, interpret them, and serve static files (like HTML, CSS, and images) from a local directory.

## Features
- Handles HTTP Requests: The server listens on a specified port and accepts incoming HTTP requests.
- **Supports GET Method:** The server currently supports the GET method for retrieving files from the server.
- **Static File Serving:** Serve static files (HTML, CSS, JavaScript, images) to the client.
- **Basic HTTP Response Handling:** Send basic HTTP responses, including headers (e.g., `200 OK` for successful requests).
- **Multi-threaded:** Supports handling multiple client connections simultaneously using threading.

## Installation
To compile and run the web server on your local machine, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/raghavayushman/web-server-c.git
   cd web-server-c
   ```

2. Compile the source code:
   ```bash
   gcc -o webserver webserver.c -lpthread
   ```

3. Run the server:
   ```bash
   ./webserver
   ```

   The server will start and listen on port 8080 by default.

4. Access the web server in your browser by navigating to `http://localhost:8080`.

## Usage
Once the server is running, you can test it by navigating to any supported file within the directory. For example:

- `http://localhost:8080/index.html`
- `http://localhost:8080/styles.css`

If the requested file exists in the server's root directory, it will be served. Otherwise, the server will return a `404 Not Found` error.

## Customization
You can modify the server to suit your needs by:
- Changing the port number in the source code.
- Adding additional HTTP methods.
- Enhancing error handling.
- Supporting dynamic content generation (e.g., integrating with a backend language).

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

This project serves as a simple, educational example of how web servers work under the hood. It's a great starting point for learning about networking, HTTP, and multi-threading in C.
