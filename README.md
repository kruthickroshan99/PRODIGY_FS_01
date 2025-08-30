# Secure Authentication System

## Description

Create a comprehensive user authentication system with secure login and registration functionality. The program allows users to sign up for accounts, log in securely, and access protected routes only after successful authentication. The system includes password hashing, session management, role-based access control, and password reset functionality. For example, if a user registers as an admin, they get access to all administrative features, while regular users only see general content.

## Features

• **User Input Handling** - Secure form validation and input sanitization
• **Password Security** - SHA-256 password hashing with strength validation
• **Session Management** - Secure session creation with automatic expiration
• **Role-Based Access Control** - Three-tier permission system (User, Moderator, Admin)
• **Password Reset** - Self-service password recovery functionality
• **Protected Routes** - Content access based on authentication status
• **Real-time Validation** - Instant feedback on form inputs and password strength
• **Responsive Design** - Modern UI that works on desktop and mobile devices

## Installation and Usage

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/secure-auth-system.git
   ```

2. Open the application:
   ```
   Open index.html in your web browser
   ```

3. Start using the authentication system with the default admin account or create your own account.

## Default Credentials

For testing purposes, use these default credentials:

**Admin Account:**
- Email: `admin@example.com`
- Password: `password`

## User Roles

| Role | Permissions |
|------|-------------|
| **User** | Access to general content only |
| **Moderator** | Access to moderation tools + general content |
| **Admin** | Full access to all content and administration |

## Security Features

- **Password Hashing**: Secure SHA-256 password hashing
- **Session Management**: 24-hour session expiration with validation
- **Input Validation**: Email format validation and required field checks
- **Password Strength**: Real-time password strength indicator
- **Role-Based Access**: Content visibility based on user permissions
- **Password Reset**: Secure password recovery without current password

## API Endpoints (Frontend Only)

This is a frontend-only demonstration. In production, you would implement these backend endpoints:

- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout
- `POST /api/auth/reset-password` - Password reset
- `GET /api/auth/profile` - Get user profile
- `PUT /api/auth/change-password` - Change password

## Technology Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Security**: Web Crypto API for password hashing
- **Storage**: In-memory storage (for demo purposes)
- **Styling**: Custom CSS with modern design patterns

## Production Considerations

For production deployment, implement these security enhancements:

### Backend Security
- Replace SHA-256 with **bcrypt** for password hashing
- Use a real database (PostgreSQL, MongoDB, etc.)
- Implement proper session storage (Redis, database sessions)
- Add **JWT tokens** for stateless authentication
- Enable **HTTPS** for all communications

### Additional Security
- **Rate limiting** for login attempts
- **CSRF protection** tokens
- **Input sanitization** and SQL injection prevention
- **Email verification** for registration
- **Two-factor authentication** (2FA)
- **Account lockout** after failed attempts

### Monitoring & Logging
- **Audit logs** for authentication events
- **Failed login monitoring**
- **Session tracking** and analytics

## Screenshots

### Login Page
![Login Interface](<img width="1919" height="910" alt="image" src="https://github.com/user-attachments/assets/554d2ead-686c-4e1d-8c2f-bbef08083b60" />
)

### Registration Form
![Registration Form](<img width="1919" height="913" alt="image" src="https://github.com/user-attachments/assets/99428eac-8b25-4f1e-bc0b-2419266c7334" />
)

### Dashboard
![User Dashboard](d5ecfa01-9a1c-42c8-b071-96f0c52f7069
)

### Password Reset
![Password Reset](<img width="1919" height="913" alt="Screenshot 2025-08-30 133646" src="https://github.com/user-attachments/assets/4e378f23-8055-4915-af8c-109d6ce863bb" />

)

---
