# The goal of this repo is explaining basics of `HTTP` with some interview questions

## What is HTTP?
 HTTP ((Hypertext Transfer Protocol) is a protocol used for communication between web browsers and web servers. It defines how requests from clients (such as browsers) are made and how servers respond to those requests. Let's break it down:
 
* HTTP Basics: HTTP is a request-response protocol, which means a client sends a request to a server, and the server responds with a corresponding response.

* URL: URLs (Uniform Resource Locators) are used to identify resources on the web. They typically consist of a scheme (e.g., "http://" or "https://"), followed by the domain name or IP address of the server, and the path to the resource.

Example: `http://www.example.com/index.html`

* HTTP Verbs (Methods): HTTP requests are made using different verbs or methods, which indicate the action the client wants to perform. The common HTTP methods are:

   * GET: Retrieves a resource from the server.

   * POST: Sends data to the server to create a new resource.

   * PUT: Sends data to the server to update or replace an existing resource.

   * DELETE: Deletes a specified resource on the server.

* HTTP Request Structure: An HTTP request consists of a request line, headers, and an optional body. Let's look at an example of a GET request:

```javascript

GET /index.html HTTP/1.1
Host: www.example.com
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.93 Safari/537.36

```

   * The first line contains the HTTP method (GET), the path of the resource (/index.html), and the HTTP version (HTTP/1.1).
   * The headers provide additional information about the request, such as the host and user agent.

* HTTP Response Structure: An HTTP response consists of a status line, headers, and an optional body. Here's an example of an HTTP response:

```javascript

HTTP/1.1 200 OK
Content-Type: text/html
Content-Length: 1274

<!DOCTYPE html>
<html>
<head>
<title>Example Page</title>
</head>
<body>
<h1>Welcome to Example Page</h1>
</body>
</html>

```

   * The first line contains the HTTP version, followed by the status code and reason phrase (200 OK indicates a successful response).

   * The headers provide additional information about the response, such as the content type and length.

   * The body contains the actual content of the response, such as HTML in this example.

* Status Codes: HTTP status codes indicate the outcome of a request. Here are a few examples:

   * 200 OK: The request was successful.
   * 404 Not Found: The requested resource was not found.
   * 500 Internal Server Error: An error occurred on the server.

