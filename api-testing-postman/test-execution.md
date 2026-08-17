# API Test Execution

This document contains the results of basic manual API testing performed using Postman.

## Test Execution Summary

| TC ID | Method | Scenario | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|
| API-001 | GET | Verify existing user details | 200 OK with user details | 200 OK with user details | Pass |
| API-002 | GET | Verify non-existing user | 404 Not Found | 404 Not Found | Pass |
| API-004 | POST | Create user with valid data | User should be created successfully | User created with generated ID | Pass |
| API-005 | POST | Create user without mandatory field | API should reject invalid request | API accepted request | Fail |
| API-006 | PUT | Update complete user data | User details should be updated | Updated data should be validated | Pending |
| API-007 | PATCH | Update only username | Only username should change | Updated field and unchanged fields should be validated | Pending |
| API-008 | DELETE | Delete user | User should be deleted successfully | 204 No Content received | Pass |

## API-001 – GET Existing User

### Request

```text
GET /users/1
