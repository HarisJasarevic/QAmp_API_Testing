Assignment 1

Investigate Restful Booker API service and create Smoke Test: https://restful-
booker.herokuapp.com/

- Explore the API and read documentation.

- Identify what you think represents a Smoke Test

- Use Postman to implement the Smoke Test (Create a collection with all steps 
covered for Smoke Test)

Note: Remember to avoid sharing your personal credentials on GitHub 
repositories 

Smoke Test Scenario for website https://restful-booker.herokuapp.com

**Smoke Test Scenario 

ID: STS-001 

Test case: TC-001** 

Description: 

This request is sent in order to check API responsiveness of the page and authentification of user in order to create Auth 
Token that we'll use in further testing for authentication.


baseURL endpoint is /auth 

For this test we provided valid email and password variables saved in Booking_App_Environment.

Expected response: 200 OK, Authentication Token generated 

Actual response: 200 OK, Authentication Token generated 

Authentication token is saved in Booking_App_Environment as accessToken variable for further testing use.



**Smoke Test Scenario

ID: SCS-001

Test case: TC-002**

Description:

This request is sent in order to create a new booking.

baseURL endpoint is /booking

For this test we provided valid info based on API documentation

Expected response: 200 OK, Booking created with provided info

Actual response: 200 OK, Booking created with provided info


**Smoke Test Scenario

ID: SCS-001

Test case: TC-003**

Description:

This request is sent in order to get booking info by it's ID.

baseURL endpoint is /booking/:bookId

For this test we provided valid ID of booking we already created trough Path variable "bookId"

Expected response: 200 OK, get booking information for requested ID

Actual response: 200 OK, get booking information for requested ID


**Smoke Test Scenario

ID: SCS-001

Test case: TC-004**

Description:

This request is sent in order to update requested booking ID information.

baseURL endpoint is /booking/:id

For this test we provided valid ID of booking we already created trough Path variable "id"

Expected response: 200 OK, updated booking information for requested ID

Actual response: 200 OK, updated booking information for requested ID



**Smoke Test Scenario

ID: SCS-001

Test case: TC-005**

Description:

This request is sent in order to delete requested booking by it's ID

baseURL endpoint is /booking/bookingID

For this test we provided valid ID of booking we already created

Expected response: 200 OK

Actual response: 200 OK