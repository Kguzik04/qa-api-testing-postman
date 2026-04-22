# Test Cases: API Testing

## Test Case 1: Get Users List
**Steps:**
1. Send GET request to `/api/users?page=2`
2. Check the response status code.
3. Verify the structure of the JSON response.

**Expected Results:**
- Status code is 200 OK.
- Response contains a list of users.
- Pagination data is correct.

---

## Test Case 2: User Login
**Steps:**
1. Send POST request to `/api/login` with valid credentials.
2. Check the response status code.

**Expected Results:**
- Status code is 200 OK.
- Response contains a "token".
