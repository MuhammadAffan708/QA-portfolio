
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


