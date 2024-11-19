# The Waiter

This project is a Node.js-based web application designed to handle user submissions through a contact form. It includes functionality to send templated emails and manage user input efficiently while adhering to specific requirements.

---

## Features

- **Contact Form**: A user-friendly form for submitting queries, including:
  - First Name and Last Name
  - Email Address
  - Query Type (General Enquiry, Support Request)
  - Message
  - Consent Checkbox
  
- **Email Notification**: Automatically sends a templated email to a specified email address upon form submission.

- **Database Cleanup**: After the email is successfully sent, all related database records are securely deleted to maintain data privacy.

---

## Requirements

- **Technology Stack**:
  - Node.js
  - Web Application Framework (e.g., Express.js)
  - Deployment to **Azure** or **AWS**

- **Deployment Environment**:
  - Azure or AWS hosting for scalability and reliability.

---

## Getting Started

### Prerequisites

- Node.js installed
- Azure or AWS account for deployment
- SMTP server details for email sending

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <project-directory>
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   - Create a `.env` file in the root directory.
   - Define the following variables:
     ```env
     EMAIL_HOST=<your-smtp-host>
     EMAIL_PORT=<smtp-port>
     EMAIL_USER=<your-email-username>
     EMAIL_PASS=<your-email-password>
     DATABASE_URL=<your-database-url>
     ```

4. Run the application:
   ```bash
   npm start
   ```

---

## Deployment

1. **Azure Deployment**:
   - Use Azure App Service or a virtual machine to host the application.
   - Configure environment variables in the Azure portal.

2. **AWS Deployment**:
   - Deploy using AWS Elastic Beanstalk or an EC2 instance.
   - Configure environment variables via the AWS Management Console.

---

## OBS (Observation)

The database storing form submissions is **deleted** after each email is sent. This ensures compliance with data privacy standards.

---

## License

This project is licensed under the [MIT License](LICENSE).

---
