# API Bug Report

## Title
GET /users returns 500 Internal Server Error for valid request

## Environment
- API Version: v1
- Tool: Postman
- Method: GET

## Steps to Reproduce
1. Open Postman
2. Send GET request to /users
3. Observe the response

## Expected Result
API returns status code 200 and a valid list of users

## Actual Result
API returns status code 500 Internal Server Error

## Severity
High

## Priority
High

## Notes
This issue blocks validation of user data and indicates a backend failure for a valid request.
