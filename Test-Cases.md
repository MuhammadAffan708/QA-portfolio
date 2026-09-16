## TC-001 — Verify Email OTP Delivery

*Test Scenario:* Verify that an OTP is delivered to the user's email after entering a valid email address.

*Preconditions:*
- NayaPay app is installed.
- User has a valid email address.
- Device is connected to the internet.

*Test Data:*
- Valid email address

*Test Steps:*
1. Open the NayaPay application.
2. Enter a valid email address.
3. Submit the email address.
4. Check the email inbox for the OTP.

*Expected Result:*
An OTP should be delivered to the entered email address, allowing the user to continue the verification process.

*Actual Result:*
OTP email was not received.

*Status:* Failed

*Related Bug:* BUG-001 — Email OTP Not Received
