## Learning JWT Token verification on register.

### Problems faced and solutions during project

- MongoDB configuration problem using **mongoose**.
  - Mongoose has issues to connect to `mongodb://localhost:27017/jwtTest`
  - Instead use `mongodb://127.0.0.1:27017/jwtTest`
- Code issue saying
  - Error [ERR_HTTP_HEADERS_SENT]: Cannot set headers after they are sent to the client
  - Issue due to logical error, where `return;` not used after a single response is returned, and thus trying to return multiple responses.

### TODO

- Add a client application for verification of the backend.
- Add more routes to create a weather api
