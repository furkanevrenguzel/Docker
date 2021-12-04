When an HTTP GET request is sent with Python Flask, "Hello World from Flask!" I developed an application whose response is returned. It runs from port 4444 in the Docker container of the application and responds to requests from the/internship path.

When an HTTP GET request is sent with Node.JS, "Hello World from Node.JS!" I developed an application whose response is returned. It responds to requests from port 5555 and/internship path in the Docker container of the application.

These applications are accessed via HAProxy running on port 8888 in another Docker container. In the HAProxy configuration, requests from the/flask path are directed to the Flask container, and the requests to the / nodejs path are directed to the Node.JS container.
