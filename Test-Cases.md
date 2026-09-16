
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

# Test Case — Email Address Format Validation

## Test Case Information

| Field         | Details                                                                                                              |
| ------------- | -------------------------------------------------------------------------------------------------------------------- |
| Test Case ID  | TC-EMAIL-002                                                                                                         |
| Test Scenario | Verify email address format validation                                                                               |
| Module        | Email Verification                                                                                                   |
| Test Type     | Functional / Negative Testing                                                                                        |
| Priority      | High                                                                                                                 |
| Related Bug   | [Bug #002 — Invalid Email Address Format Accepted](../Bug-Reports.md#bug-002--invalid-email-address-format-accepted) |

## Preconditions

* User is on the email verification screen.
* Email input field is available.
* Application is connected to the internet.

## Test Data

**Invalid Email:**

`test@example.com.`

The email address contains an invalid trailing dot in the domain portion.

## Test Steps

| Step | Action                                        | Expected Result                                                                 | Actual Result                                                                | Status |
| ---- | --------------------------------------------- | ------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ------ |
| 1    | Open the email verification screen.           | Email input field should be displayed.                                          | Email input field is displayed.                                              | Pass   |
| 2    | Enter `test@example.com.` in the email field. | System should identify the email address as invalid.                            | Application accepts the email address.                                       | Fail   |
| 3    | Click **Continue / Submit**.                  | System should display an appropriate validation message and prevent submission. | Application accepts the email address instead of showing a validation error. | Fail   |

## Expected Result

The application should validate the email address according to standard email formatting rules and reject invalid email formats.

## Actual Result

The application accepts an email address containing an invalid trailing dot in the domain portion instead of displaying a validation error.

## Test Result

**Status:** Failed

## Defect Reference

[View Bug #002 — Invalid Email Address Format Accepted](../Bug-Reports.md#bug-002--invalid-email-address-format-accepted)


