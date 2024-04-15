a# Generate CSRF PoC

Author: RyotaK

Workflow to generate CSRF PoC from the request. Currently, only `application/x-www-form-urlencoded` and `application/json` (with the `text/plain` technique) are supported.

## Usage
Convert the whole request using this workflow like the following:
```
POST / HTTP/1.1
Host: example.com
Content-Type: application/x-www-form-urlencoded

name=value
```

If the application only listens on HTTP, please change the protocol to `http` in the generated PoC.  