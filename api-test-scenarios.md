# API Test Scenarios

## Endpoint
GET /users

## Positive Test Cases

### TC-001: Verify successful response
- Send GET request to /users
- Expected status code: 200
- Expected result: Response returns a list of users

### TC-002: Verify response format
- Send GET request to /users
- Expected result: Response content type is application/json

### TC-003: Verify required fields
- Send GET request to /users
- Expected result: Each user object includes expected fields such as id, name, and email

## Negative Test Cases

### TC-004: Invalid endpoint
- Send GET request to /invalid-users
- Expected status code: 404
- Expected result: Error message is returned

### TC-005: Unauthorized request
- Send request without valid authorization
- Expected status code: 401 or 403
- Expected result: Access is denied with appropriate error message

### TC-006: Invalid query parameter
- Send request with unsupported query parameter
- Expected result: API handles request gracefully and returns proper validation or error response
