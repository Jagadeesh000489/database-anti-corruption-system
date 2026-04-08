
# Anti-Corruption Reporting Portal

This is a web application for anonymously reporting corruption incidents. The application includes a frontend built with React and a backend built with PHP and MySQL.

## Features

- User authentication via email/phone and password
- OTP generation for enhanced security
- Comprehensive complaint form with multiple sections
- Evidence upload functionality
- Confidentiality options
- Responsive design for all devices

## Setup Instructions

### Prerequisites

- Node.js and npm
- PHP 7.4 or higher
- MySQL 5.7 or higher
- Web server (Apache, Nginx, etc.)

### Frontend Setup

1. Clone the repository
2. Install dependencies:
   ```
   npm install
   ```
3. Start the development server:
   ```
   npm run dev
   ```

### Backend Setup

1. Configure your web server to point to the `public` directory
2. Import the database schema:
   - The schema is automatically created when you first access the application
   - You can also manually import the schema using the SQL in `src/db_config.php`
3. Update database configuration in `src/db_config.php` if needed

### File Uploads

1. Create a directory named `uploads` in the root directory
2. Make sure the directory has write permissions:
   ```
   chmod 755 uploads
   ```

## Project Structure

- `/src` - React frontend code
- `/public` - Public assets and PHP backend scripts
- `/src/pages` - React page components
- `/src/components` - Reusable React components
- `/uploads` - Directory for uploaded files (created automatically)

## API Endpoints

- `signin.php` - Handles user authentication
- `generate_otp.php` - Generates OTP for login
- `submit_complaint.php` - Processes complaint form submissions

## Security Considerations

- This is a demo application and should not be used in production without additional security measures
- In a production environment, you should:
  - Use HTTPS for all communications
  - Implement proper password hashing
  - Add rate limiting to prevent abuse
  - Implement CSRF protection
  - Add proper input validation and sanitization

## License

# Database Design – Anti-Corruption Reporting System

## Overview
This project focuses on designing and managing a MySQL database for storing complaint and user data.

## Tools Used
- MySQL

## Key Work
- Designed database schema (tables, relationships)
- Wrote SQL queries (JOIN, GROUP BY)
- Managed and stored structured data
- Ensured data accuracy and consistency

This project is licensed under the MIT License - see the LICENSE file for details.
