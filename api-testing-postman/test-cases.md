# API Testing Test Cases

This document contains manual API testing test cases executed using Postman.

## Test Cases

| TC ID | Method | Test Scenario | Expected Result |
|---|---|---|---|
| API-001 | GET | Verify API returns valid data | API should return 200 OK with valid response data |
| API-002 | GET | Verify invalid endpoint | API should return 404 Not Found |
| API-003 | GET | Verify response body | Response should contain the expected fields and values |
| API-004 | POST | Verify user creation with valid data | API should create the user successfully |
| API-005 | POST | Verify user creation with invalid data | API should return an appropriate validation/error response |
| API-006 | PUT | Verify updating complete user data | API should update the requested resource successfully |
| API-007 | PATCH | Verify updating a single field | Only the specified field should be updated |
| API-008 | DELETE | Verify deleting a resource | API should delete the requested resource successfully |
| API-009 | GET | Verify response headers | Response should contain the required headers |
| API-010 | GET | Verify authentication | Unauthorized request should be rejected |
| API-011 | GET | Verify response status code | Actual status code should match the expected status code |
| API-012 | GET | Verify response data accuracy | Received data should match the expected data |
