
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

# Test Case — Navbar Responsiveness on Mobile Portrait View

## Test Case Information

| Field             | Details                                                                                                                              |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **Test Case ID**  | TC-UI-001                                                                                                                            |
| **Test Scenario** | Verify navbar displays correctly on mobile portrait view                                                                             |
| **Module**        | Navigation Bar                                                                                                                       |
| **Test Type**     | UI / Responsive Testing                                                                                                              |
| **Priority**      | Medium                                                                                                                               |
| **Related Bug**   | [Bug-003 — Navbar Text Overflows on Mobile Portrait View](../Bug-Reports.md#bug-003--navbar-text-overflows-on-mobile-portrait-view) |

## Preconditions

* Website is accessible.
* Device is connected to the internet.
* Google Chrome is installed.
* Device is set to portrait orientation.

## Test Environment

| Field           | Details            |
| --------------- | ------------------ |
| **Device**      | Tecno Camon 19 Neo |
| **OS**          | Android 13         |
| **Browser**     | Google Chrome      |
| **Orientation** | Portrait           |

## Test Steps

| Step | Action                                                                | Expected Result                                                                     | Actual Result                                                | Status |
| ---- | --------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------ | ------ |
| 1    | Open the DEVFOREST AI (SMC-PRIVATE) LIMITED website in Google Chrome. | Website should load successfully.                                                   | Website loaded successfully.                                 | Pass   |
| 2    | Keep the device in portrait orientation.                              | Website should adapt correctly to the mobile viewport.                              | Website displayed in portrait mode.                          | Pass   |
| 3    | Observe the navbar and its navigation items.                          | All navbar text should remain within the navigation container and be fully visible. | A navbar text item extends outside the navigation container. | Fail   |

## Expected Result

All navbar items should remain within the navigation container and should be fully visible without overflow or layout issues on a mobile portrait viewport.

## Actual Result

A navbar text item extends outside the navigation container in portrait mode.

## Test Result

**Status: Failed**

## Defect Reference

[View Bug-003 — Navbar Text Overflows on Mobile Portrait View](../Bug-Reports.md#bug-003--navbar-text-overflows-on-mobile-portrait-view)







