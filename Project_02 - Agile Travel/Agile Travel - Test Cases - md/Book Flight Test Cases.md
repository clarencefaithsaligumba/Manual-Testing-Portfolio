| Test Case ID | Test Cases      |                                                                                                                                   | Status        | Priority |
|--------------|-----------------|-----------------------------------------------------------------------------------------------------------------------------------|---------------|----------|
| TS_001       | Test Case Title | Validate selecting different origin and destination locations from the dropdown menu                                              |               |          |
|              | Precondition    | Ensure the user is successfully login and on the "Select Flight" page.                                                            | Ready to Test | High     |
|              | Test Steps      | 1. Select "Return" as a trip type                                                                                                 |               |          |
|              |                 | 2. Click on the "From" (Origin) drop down menu                                                                                    |               |          |
|              |                 | 3. Select a specific city from the "Origin" list (e.g., "New York")                                                               |               |          |
|              |                 | 4. Click on the "To" (Destination) drop down menu                                                                                 |               |          |
|              |                 | 5. Select a specific city from the  "Destination" list (e.g., "Sydney")                                                           |               |          |
|              |                 | 6. Set the "Departing" and "Returning" dates ensuring the return date is later than the departure date.                           |               |          |
|              |                 | 7. Click the "Continue" button                                                                                                    |               |          |
| TS_002       | Test Case Title | Validate that system allow a user to book a return flight with a return date that occurs after the departure date                 |               |          |
|              | Precondition    | Ensure the user is successfully login and on the "Select Flight" page.                                                            | Ready to Test | High     |
|              | Test Steps      | 1. Select "Return" as a trip type                                                                                                 |               |          |
|              |                 | 2. Click on the "From" (Origin) drop down menu                                                                                    |               |          |
|              |                 | 3. Select a specific city from the "Origin" list (e.g., "New York")                                                               |               |          |
|              |                 | 4. Select a specific city from the  "Destination" list (e.g., "Sydney")                                                           |               |          |
|              |                 | 5. Set the "Departing" flight date before the returning flight date (e.g., "January 1, 2026")                                     |               |          |
|              |                 | 6. Set the "Returning" flight date after the departing flight date (e.g., "January 10, 2026")                                     |               |          |
|              |                 | 7. Select a "Time Flight No." (e.g., "8:00 QF821")                                                                                |               |          |
|              |                 | 8. Click the "Continue" button                                                                                                    |               |          |
| TS_003       | Test Case Title | Validate the booking must proceed to the next page when all required fields are filled and the continue button is clicked         |               |          |
|              | Precondition    | Ensure the user is successfully login and on the "Select Flight" page.                                                            | Ready to Test | High     |
|              | Test Steps      | 1. Select "Return" as a trip type                                                                                                 |               |          |
|              |                 | 2. Fill out all the mandatory fields (From, To, Departing, Returning, Time Flight No.) in the "Select Flight" page                |               |          |
|              |                 | 3. Click the "Continue" button                                                                                                    |               |          |
| TS_004       | Test Case Title | Validate booking should display error or not prevent a user to redirect to the next page if the departure date is set in the past |               |          |
|              | Precondition    | Ensure the user is successfully login and on the "Select Flight" page.                                                            | Ready to Test | High     |
|              | Test Steps      | 1. Select "Return" as a trip type                                                                                                 |               |          |
|              |                 | 2. Fill out all the mandatory fields (From, To, Departing, Returning, Time Flight No.) in the "Select Flight" page                |               |          |
|              |                 | 3. Select a past date for the "Departing" field (e.g., March 1, 2016) to verify date validation logic                             |               |          |
|              |                 | 4. Click the "Continue" button                                                                                                    |               |          |
| TS_005       | Test Case Title | Validate that when selecting a one-way trip should successfully disable or hide the returning date selection fields               |               |          |
|              | Precondition    | Ensure the user is successfully login and on the "Select Flight" page.                                                            | Ready to Test | Medium   |
|              | Test Steps      | 1. Select "One way" as a trip type                                                                                                |               |          |
|              |                 | 2. Observe the "Returning" date selection fields.                                                                                 |               |          |
| TS_006       | Test Case Title | Validate booking should display error if the user set a returning date that is earlier than the departing date                    |               |          |
|              | Precondition    | Ensure the user is successfully login and on the "Select Flight" page.                                                            | Ready to Test | Medium   |
|              | Test Steps      | 1. Select "Return" as a trip type                                                                                                 |               |          |
|              |                 | 2. Click on the "From" (Origin) drop down menu                                                                                    |               |          |
|              |                 | 3. Select a specific city from the "Origin" list (e.g., "New York")                                                               |               |          |
|              |                 | 4. Select a specific city from the  "Destination" list (e.g., "Sydney")                                                           |               |          |
|              |                 | 5. Set the "Departing" flight date before the returning flight date (e.g., "January 10, 2026")                                    |               |          |
|              |                 | 6. Set the "Returning" flight date after the departing flight date (e.g., "January 1, 2026")                                      |               |          |
|              |                 | 7. Select a "Time Flight No." (e.g., "8:00 QF821")                                                                                |               |          |
|              |                 | 8. Click the "Continue" button                                                                                                    |               |          |
| TS_007       | Test Case Title | Validate booking should prevent the user from booking a flight where the origin and destination are the same city                 |               |          |
|              | Precondition    | Ensure the user is successfully login and on the "Select Flight" page.                                                            | Ready to Test | Medium   |
|              | Test Steps      | 1. Select "Return" as a trip type                                                                                                 |               |          |
|              |                 | 2. Click on the "From" (Origin) drop down menu                                                                                    |               |          |
|              |                 | 3. Select the same city for both "Origin" and "Destination" fields (e.g., "New York").                                            |               |          |
|              |                 | 4. Click the "Continue" button                                                                                                    |               |          |
| TS_008       | Test Case Title | Validate booking should display error if the user tries to click "Continue" button without selecting a origin or destination      |               |          |
|              | Precondition    | Ensure the user is successfully login and on the "Select Flight" page.                                                            | Ready to Test | Lowest   |
|              | Test Steps      | 1. Select "Return" as a trip type                                                                                                 |               |          |
|              |                 | 2. Fill out all the mandatory fields except "From" and "To" fields in the "Select Flight" page                                    |               |          |
|              |                 | 3. Click the "Continue" button                                                                                                    |               |          |
