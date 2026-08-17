# Test Execution Report

## Overview

This document contains test execution results for the manual testing activities performed on the application.

## Test Execution Summary

| Metric | Count |
|---|---:|
| Total Test Cases | 10 |
| Passed | 7 |
| Failed | 2 |
| Blocked | 1 |
| Not Executed | 0 |

## Test Execution Details

| TC ID | Test Scenario | Expected Result | Actual Result | Status | Defect ID |
|---|---|---|---|---|---|
| TC-001 | Verify valid login | User should be logged in successfully | User logged in successfully | Pass | - |
| TC-002 | Verify invalid password | Error message should be displayed | Error message displayed | Pass | - |
| TC-003 | Verify empty mobile number | Validation message should be displayed | Validation message displayed | Pass | - |
| TC-004 | Verify invalid mobile number | Appropriate validation message should be displayed | Validation message displayed | Pass | - |
| TC-005 | Verify logout | User should be logged out successfully | User logged out successfully | Pass | - |
| TC-006 | Verify login with expired OTP | User should not be logged in | User was not logged in | Pass | - |
| TC-007 | Verify login button with invalid data | Login should not proceed | Login button allowed navigation | Fail | BUG-001 |
| TC-008 | Verify OTP resend | New OTP should be generated | OTP was not received | Fail | BUG-002 |
| TC-009 | Verify login under network interruption | Appropriate network error should be displayed | API request remained loading | Blocked | BUG-003 |
| TC-010 | Verify successful login navigation | User should be redirected to Home | User redirected to Home | Pass | - |

## Defect Summary

| Defect ID | Description | Severity | Status |
|---|---|---|---|
| BUG-001 | Login proceeds with invalid input | High | Open |
| BUG-002 | OTP not received after resend | High | Open |
| BUG-003 | Login remains loading during network interruption | Medium | Open |

## Test Environment

- Application: Sample Mobile Application
- Platform: Android
- Environment: QA / Staging
- Testing Type: Manual Testing
- Browser: Chrome
- Network: Wi-Fi / Mobile Data

## Testing Types Covered

- Functional Testing
- Positive Testing
- Negative Testing
- UI Testing
- Validation Testing
- Regression Testing
- Smoke Testing
- Sanity Testing

## Execution Result

The majority of the executed test cases passed successfully. The failed and blocked scenarios were documented as defects for further investigation and resolution.

## Conclusion

Test execution was completed for the selected functionality. Identified defects have been documented with severity and status for tracking and retesting.
