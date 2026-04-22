# Bug Report: Missing Password in Login

**Bug ID:** BUG-001
**Status:** Open
**Severity:** Medium

**Description:**
When sending a POST request to `/api/login` without a password field, the system returns an unhelpful error or wrong status code.

**Steps to Reproduce:**
1. Open Postman.
2. Set method to POST and URL to `https://reqres.in/api/login`.
3. In Body, provide only `"email": "eve.holt@reqres.in"`.
4. Send request.

**Expected Result:**
Status code 400 Bad Request with message "Missing password".

**Actual Result:**
Status code 400 Bad Request, but error message is generic.
