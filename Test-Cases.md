
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
