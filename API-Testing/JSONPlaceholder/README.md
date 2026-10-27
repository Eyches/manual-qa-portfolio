# JSONPlaceholder — API Testing Mini-case

## Project Overview

This project demonstrates basic REST API testing using Postman and the public JSONPlaceholder API.

The objective was to design and execute positive and negative API tests, validate HTTP responses, and document the results.

**API:** https://jsonplaceholder.typicode.com/  
**Tool:** Postman  
**Testing Date:** 2026-10-27  
**Testing Type:** Manual API Testing with Postman Assertions

## Test Scope

Two GET requests were tested:

| Test Case | Endpoint | Expected Status | Actual Status | Result |
|---|---|---|---|---|
| Get existing post | `/posts/5` | 200 OK | 200 OK | PASSED |
| Get non-existing post | `/posts/99999` | 404 Not Found | 404 Not Found | PASSED |

## Assertions

**Positive Test — GET /posts/5**

- HTTP Status Code equals 200.
- Post `id` equals 5.
- `title` is a string.
- `body` is a non-empty string.

**Negative Test — GET /posts/99999**

- HTTP Status Code equals 404.
- Response Body is an empty JSON object (`{}`).

## Test Results

- Total Requests: 2
- Total Assertions: 6
- Passed: 6
- Failed: 0

Results are based on manual execution and observation in Postman.

## How to Run

1. Open Postman.
2. Import the included `.postman_collection.json` file.
3. Open the imported collection.
4. Run each request using **Send**.
5. Review the assertion results in the Postman response panel.

## Testing Limitations

- Only GET requests were tested.
- POST, PUT, PATCH and DELETE were not covered.
- The `userId` value was not validated in this mini-case.
- The actual text content of `title` and `body` was not validated.
- Response time was not validated against a performance requirement.
- Authentication, authorization, and additional invalid-input scenarios were not tested.

## Conclusion

Both documented API requests passed all six assertions during testing.

This mini-case demonstrates basic positive and negative API testing, JSON response validation, and Postman scripting.

The limited scope does not establish that the complete API is defect-free.
