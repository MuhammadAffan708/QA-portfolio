
# Test Case: Email OTP Delivery

**Test Case ID:** TC-001

**Test Scenario:** Verify that an OTP is delivered to the user's email after entering a valid email address.

**Module:** Email Verification

**Priority:** High

**Preconditions:**
- NayaPay app is installed.
- User has a valid email address.
- Device is connected to the internet.

**Test Data:**
- Valid email address

**Test Steps:**

| Step No. | Test Step | Expected Result |
|---|---|---|
| 1 | Open the NayaPay application. | NayaPay application opens successfully. |
| 2 | Enter a valid email address. | Email address is accepted. |
| 3 | Submit the email address. | OTP verification process is initiated. |
| 4 | Check the email inbox for the OTP. | OTP email should be received. |

**Expected Result:**

An OTP should be delivered to the entered email address, allowing the user to continue the verification process.

**Actual Result:**

OTP email was not received.

**Status:** Failed

**Related Bug:** BUG-001 — Email OTP Not Received


## TC-002 — Verify Invalid Email Format Validation
*Related Bug:* [BUG-002 — Invalid Email Format Accepted](./Bug-Reports.md#bug-002--invalid-email-format-accepted)

*Test Scenario:* Verify that the application rejects an invalid email address format.

*Preconditions:*
- NayaPay app is installed.
- User is on the email verification screen.
- Device is connected to the internet.

*Test Data:*
- Invalid email: aaaaaaaaaa{}*"&*/_+$#@gmail.com

*Test Steps:*
1. Open the NayaPay application.
2. Navigate to the email verification screen.
3. Enter the invalid email address aaaaaaaaaa{}*"&*/_+$#@gmail.com.
4. Tap the *Next* button.
5. Observe the application response.

*Expected Result:*
The application should reject the invalid email format and display an appropriate validation message.

*Actual Result:*
To be recorded after test execution.

*Status:* Not Executed






