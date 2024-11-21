## Features

- **OTP Generation:** Automatically generates a secure 6-digit OTP for user authentication, ensuring randomization and unpredictability.
- **Email Integration:** Delivers the generated OTP to the user's email address via an automated Gmail SMTP integration.
- **Verification Process:** Provides the user with a maximum of three attempts to enter the correct OTP, with automated input validation for enhanced security.

## How It Works

1. **User Input:** The user is prompted to enter their email address to initiate the OTP process.
2. **OTP Generation:** The system generates a secure, random 6-digit OTP using Python’s `random.choices()` function, ensuring each OTP is unique.
3. **OTP Delivery:** The generated OTP is automatically transmitted to the user's email via a secure SMTP connection to Gmail, eliminating the need for manual intervention.
4. **OTP Verification:** The user is prompted to input the OTP received via email. The system automatically validates the entered OTP, allowing up to three attempts to ensure accuracy.
5. **Result:**
   - If the OTP entered matches the generated code, the user is successfully authenticated.
   - After three failed attempts, the system automatically locks the process and prompts the user to retry later.

## Automation Overview:

- **OTP Generation:** The OTP is generated through a fully automated process using Python’s `random.choices()` function, ensuring each OTP is randomly created and secure for every session.
- **Email Delivery:** The OTP is sent automatically via the `smtplib` library and Gmail’s SMTP server, streamlining the communication process without manual effort.
- **Verification Process:** The entire validation workflow, including user input validation and multiple attempts, is automated, reducing human intervention and enhancing the efficiency and security of the authentication procedure.

