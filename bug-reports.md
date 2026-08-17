# Manual Testing - Bug Reports

## Bug Report 001

| Field | Details |
|---|---|
| Bug ID | BUG-001 |
| Bug Title | Login fails with valid credentials |
| Module | Login |
| Severity | Critical |
| Priority | High |
| Environment | Android / Production |
| Status | Open |

### Preconditions
- User has a registered account.
- User has valid login credentials.
- Application is installed and launched.

### Steps to Reproduce
1. Open the application.
2. Navigate to the Login screen.
3. Enter a valid registered email/phone number.
4. Enter the correct password.
5. Tap the **Login** button.

### Expected Result
User should be successfully logged in and redirected to the Home screen.

### Actual Result
User remains on the Login screen and is not logged in.

---

## Bug Report 002

| Field | Details |
|---|---|
| Bug ID | BUG-002 |
| Bug Title | Login button remains enabled with empty fields |
| Module | Login |
| Severity | Medium |
| Priority | Medium |
| Environment | Android / Production |
| Status | Open |

### Steps to Reproduce
1. Open the application.
2. Navigate to the Login screen.
3. Leave the email/phone field empty.
4. Leave the password field empty.
5. Observe the Login button.

### Expected Result
Login button should remain disabled until mandatory fields are entered.

### Actual Result
Login button remains enabled and can be tapped.

---

## Bug Report 003

| Field | Details |
|---|---|
| Bug ID | BUG-003 |
| Bug Title | Incorrect error message displayed for invalid password |
| Module | Login |
| Severity | Medium |
| Priority | Medium |
| Environment | Android / Production |
| Status | Open |

### Steps to Reproduce
1. Open the application.
2. Enter a valid registered email/phone number.
3. Enter an incorrect password.
4. Tap **Login**.

### Expected Result
A clear error message such as **"Invalid password"** should be displayed.

### Actual Result
A generic or incorrect error message is displayed.

---

## Bug Report 004

| Field | Details |
|---|---|
| Bug ID | BUG-004 |
| Bug Title | Login button can be clicked multiple times during login request |
| Module | Login |
| Severity | High |
| Priority | High |
| Environment | Android / Production |
| Status | Open |

### Steps to Reproduce
1. Open the Login screen.
2. Enter valid credentials.
3. Tap the **Login** button repeatedly before the request completes.
4. Observe the application behavior.

### Expected Result
The Login button should be disabled or show a loading indicator until the login request is completed.

### Actual Result
The button can be clicked multiple times, potentially triggering multiple login requests.

---

## Bug Report 005

| Field | Details |
|---|---|
| Bug ID | BUG-005 |
| Bug Title | Password is visible while entering password |
| Module | Login |
| Severity | Medium |
| Priority | Medium |
| Environment | Android / Production |
| Status | Open |

### Steps to Reproduce
1. Open the Login screen.
2. Tap the Password field.
3. Enter a password.
4. Observe the entered password.

### Expected Result
Password characters should be masked for security.

### Actual Result
Password characters are visible to the user.

---

## Bug Summary

| Bug ID | Severity | Priority | Status |
|---|---|---|---|
| BUG-001 | Critical | High | Open |
| BUG-002 | Medium | Medium | Open |
| BUG-003 | Medium | Medium | Open |
| BUG-004 | High | High | Open |
| BUG-005 | Medium | Medium | Open |
