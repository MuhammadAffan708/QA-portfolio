
# BUG-001 — Email OTP Not Received

## Bug Information

| Field | Details |
|---|---|
| Bug ID | BUG-001 |
| Title | Email OTP Not Received |
| Application | NayaPay |
| Feature | Email OTP Verification |
| Severity | High |
| Priority | High |
| Status | Open — Requires Investigation |
| Reproducibility | Reproduced multiple times |

## Environment

| Environment | Details |
|---|---|
| Device | Tecno Camon 19 Neo |
| Operating System | Android 13 |
| Application Version | 3.7.7 |
| Network | Wi-Fi |

## Description

After entering a valid email address, the application displays the message "OTP has been sent to your mail." However, the OTP email is not received in the corresponding email account, preventing the user from continuing the verification process.

## Preconditions

- NayaPay application is installed.
- User has access to a valid email account.
- Device is connected to Wi-Fi.

## Steps to Reproduce

1. Open the NayaPay application.
2. Enter a valid email address.
3. Submit the email address.
4. Observe the confirmation message.
5. Open the corresponding email account.
6. Check the Inbox and Spam/Junk folders.
7. Search for NayaPay or OTP.
8. Wait for the OTP email.

## Expected Result

The OTP email should be delivered to the entered email address so the user can continue the verification process.

## Actual Result

The application displays "OTP has been sent to your mail," but the OTP email is not received.

## Reproducibility

The issue was reproduced multiple times, including with different email addresses.

## Severity

**High** — The issue prevents users from completing the email verification process.

## Priority

**High** — Investigation and resolution are required to restore the verification flow.

## Evidence

- Screen recording of the reproduction steps is available.

## Related Test Case

- TC-001 — Verify Email OTP Delivery

## Status

**Open — Requires Investigation**


https://github.com/user-attachments/assets/01287cb3-8117-48fe-9536-5744e1e317d9



# BUG-002 — Invalid Email Format Accepted

## Bug Information

| Field | Details |
|---|---|
| Bug ID | BUG-002 |
| Title | Invalid Email Format Accepted by Email Validation |
| Application | NayaPay |
| Feature | Email Validation |
| Severity | Medium |
| Priority | Medium |
| Status | Open — Requires Investigation |
| Reproducibility | Reproduced |

## Environment

| Environment | Details |
|---|---|
| Device | Tecno Camon 19 Neo |
| Operating System | Android 13 |
| Application Version | 3.7.7 |
| Network | Wi-Fi |

## Description

The NayaPay application accepts an email address containing an unquoted double quotation mark (`"`) in the local part.

According to the RFC 5322 dot-atom syntax, a double quotation mark is not permitted in an unquoted local part. The application should validate the email format and reject the invalid input.

## Preconditions

- NayaPay application is installed.
- User is on the name and email registration screen.
- Device is connected to Wi-Fi.

## Test Data

**Invalid Email Address:**

```text
aaaaaaaaaa{}*"&*/_+$##@gmail.com
```

**Validation Reference:** RFC 5322 — Email Address Syntax

## Steps to Reproduce

1. Open the NayaPay application.
2. Navigate to the name and email registration screen.
3. Enter a first name.
4. Enter a last name.
5. Enter the invalid email address:
   `aaaaaaaaaa{}*"&*/_+$##@gmail.com`
6. Observe the email input field.
7. Check whether the Next button remains enabled.

## Expected Result

The application should identify the invalid email format and display a clear validation message, such as:

> Please enter a valid email address.

The user should not be allowed to proceed with an invalid email address.

## Actual Result

The application accepts the invalid email address and the Next button remains enabled, as shown in the attached screenshot.

## Impact

Users may enter incorrectly formatted email addresses, potentially causing issues during email verification or account registration.

## Severity

**Medium** — The issue affects input validation and may allow invalid email data to proceed.

## Priority

**Medium** — The validation behavior should be reviewed and corrected.

## Evidence

https://github.com/user-attachments/assets/1b538276-d83a-48c8-8c1c-2fdb4f4b2f08

## Related Test Case

- TC-002 — Verify Invalid Email Format Validation

## Status

**Open — Requires Investigation**


# Bug #003 — Navbar Text Overflows on Mobile Portrait View

## Environment

| Field           | Details                            |
| --------------- | ---------------------------------- |
| **Website**     | DEVFOREST AI (SMC-PRIVATE) LIMITED |
| **Device**      | Tecno Camon 19 Neo                 |
| **OS**          | Android 13                         |
| **Browser**     | Google Chrome                      |
| **Orientation** | Portrait                           |
| **Test Type**   | UI / Responsive Testing            |

## Preconditions

* Website is accessible.
* Device is connected to the internet.
* Browser is using the default zoom level.

## Steps to Reproduce

1. Open the DEVFOREST AI (SMC-PRIVATE) LIMITED website in Google Chrome.
2. Hold the device in **portrait orientation**.
3. Navigate to the affected navigation section.
4. Observe the navbar text.

## Expected Result

Navbar text should remain completely within the navigation container and should be clearly visible without overflowing or overlapping other elements.

## Actual Result

The affected navbar text extends outside the navigation container when the website is viewed in portrait orientation.

## Reproducibility

**100%**

## Severity

**Low**

## Priority

**Medium**

## Status

**Open**

## Cross-Viewport Verification

| Viewport           | Result                |
| ------------------ | --------------------- |
| Mobile — Portrait  |  Issue Reproduced    |
| Mobile — Landscape |  Working as Expected |
| Desktop            | 

 Working as Expected |

## Evidence

> https://github.com/user-attachments/assets/f39f1040-e22e-454c-8135-b47fdc012946

## Notes

The issue appears to be related to the responsive layout at the narrower mobile viewport.






