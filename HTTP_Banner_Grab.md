# Send a banner grab request to an HTTP website

The `HEAD` request is apart of the Hypertext Transfer protocol. It retreives basic meta information about web servers. It makes for a simple way of getting the service and it's version number. Using a tool such as netcat, send this to the server.
```
HEAD / HTTP/1.1
```

###### https://tools.ietf.org/html/rfc7231#section-4.3.2
