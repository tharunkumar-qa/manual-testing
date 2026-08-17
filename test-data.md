# Manual Testing - Test Data

## Login Test Data

| Test Data ID | Input Type | Test Data | Expected Result |
|---|---|---|---|
| TD-001 | Email | validuser@example.com | Login should be successful |
| TD-002 | Email | invaliduser@example.com | Appropriate error message should be displayed |
| TD-003 | Email | userexample.com | Email format validation should be displayed |
| TD-004 | Email | user@ | Email format validation should be displayed |
| TD-005 | Email | @example.com | Email format validation should be displayed |
| TD-006 | Email | Empty | Mandatory field validation should be displayed |
| TD-007 | Password | ValidPassword@123 | Login should be successful with valid credentials |
| TD-008 | Password | WrongPassword@123 | Invalid credentials error should be displayed |
| TD-009 | Password | Empty | Mandatory field validation should be displayed |
| TD-010 | Password | 123 | Password validation should be displayed |

---

## Boundary Value Test Data

| Test Data ID | Field | Test Data | Purpose |
|---|---|---|---|
| TD-011 | Password | 7 characters | Verify minimum length validation |
| TD-012 | Password | 8 characters | Verify minimum valid length |
| TD-013 | Password | 15 characters | Verify valid boundary |
| TD-014 | Password | 16 characters | Verify maximum/extended length handling |
| TD-015 | Email | 1 character | Verify minimum input handling |
| TD-016 | Email | Very long email | Verify maximum input handling |

---

## Negative Test Data

| Test Data ID | Scenario | Test Data | Expected Result |
|---|---|---|---|
| TD-017 | Special characters | `<script>` | Input should be safely handled |
| TD-018 | SQL-like input | `' OR '1'='1` | Application should reject/handle input safely |
| TD-019 | Spaces | `   ` | Validation message should be displayed |
| TD-020 | Leading spaces | ` user@example.com` | Application should handle spaces correctly |
| TD-021 | Trailing spaces | `user@example.com ` | Application should handle spaces correctly |
| TD-022 | Unicode characters | `测试用户` | Application should handle input correctly |

---

## Authentication Test Data

| Test Data ID | Scenario | Username/Email | Password | Expected Result |
|---|---|---|---|---|
| TD-023 | Valid credentials | validuser@example.com | ValidPassword@123 | User should be logged in |
| TD-024 | Invalid password | validuser@example.com | WrongPassword@123 | Login should fail |
| TD-025 | Invalid username | invaliduser@example.com | ValidPassword@123 | Login should fail |
| TD-026 | Both invalid | invaliduser@example.com | WrongPassword@123 | Login should fail |
| TD-027 | Empty username | Empty | ValidPassword@123 | Username validation should be displayed |
| TD-028 | Empty password | validuser@example.com | Empty | Password validation should be displayed |
| TD-029 | Both empty | Empty | Empty | Mandatory field validations should be displayed |

---

## Test Data Categories

The following categories are covered in this document:

- Valid test data
- Invalid test data
- Boundary value data
- Empty/null values
- Special characters
- Whitespace validation
- Authentication data
- Negative test data
- Input format validation

> Note: The credentials used above are dummy test data and should not be real user credentials.
