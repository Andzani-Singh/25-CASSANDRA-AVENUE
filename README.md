# 25-CASSANDRA-AVENUE
Residence website that allow  student to register and apply for 25 Cassandra student accomodation


# Student Residence Management System

A complete PHP-based student residence management system using JSON files for data storage. Built for VUT students to find, apply for and manage student accommodation.

## Features

- **Student Registration**: Full registration with student details, funding type, and academic information
- **Login System**: Secure login with password hashing using PHP sessions
- **Residence Browsing**: Search and filter residences by price, funding type, and availability
- **Application System**: Apply for residences with detailed application forms
- **Application Tracking**: Students can track their application status (Pending, Approved, Rejected)
- **Admin Dashboard**: Complete admin panel for managing students, residences, and applications
- **Profile Management**: Students can update their profile information
- **Responsive Design**: Modern, mobile-friendly interface using CSS Grid and Flexbox

## Requirements

- PHP 7.4 or higher
- Web server (Apache, Nginx, or PHP built-in server)
- No database required (uses JSON files)

## Project Structure

```
residence-management/
├── index.php              # Homepage
├── login.php              # Login page
├── register.php           # Student registration
├── logout.php             # Logout handler
├── README.md              # This file
├── .htaccess              # (Optional) Apache configuration
│
├── admin/                 # Admin panel
│   ├── dashboard.php      # Admin dashboard
│   ├── students.php       # Manage students
│   ├── residences.php     # Manage residences
│   └── applications.php   # Manage applications
│
├── student/               # Student panel
│   ├── dashboard.php      # Student dashboard
│   ├── residences.php     # Browse residences
│   ├── apply.php          # Apply for residence
│   ├── applications.php   # View my applications
│   └── profile.php        # Manage profile
│
├── includes/              # Shared PHP files
│   ├── auth.php           # Authentication functions
│   ├── functions.php      # Helper functions
│   ├── header.php         # Site header
│   ├── footer.php         # Site footer
│   ├── admin-auth.php     # Admin authentication
│   ├── admin-header.php   # Admin header
│   └── admin-footer.php   # Admin footer
│
├── data/                  # JSON data files (PROTECTED)
│   ├── .htaccess          # Prevents direct access
│   ├── users.json         # User accounts
│   ├── residences.json    # Residence listings
│   └── applications.json  # Applications
│
├── css/                   # Stylesheets
│   └── style.css          # Main stylesheet
│
├── js/                    # JavaScript
│   └── script.js          # Main JavaScript file
│
└── images/                # Image assets
```

## Security Features

- **Password Hashing**: All passwords are hashed using `password_hash()`
- **Session Management**: Secure PHP sessions for authentication
- **Input Validation**: All inputs are sanitized and validated
- **XSS Protection**: Output is escaped using `htmlspecialchars()`
- **CSRF Protection**: Basic CSRF protection on forms
- **Data Protection**: The `data` folder is protected with `.htaccess` to prevent direct access
- **Role-Based Access**: Admin pages are protected from student access


## Browser Compatibility

- Google Chrome (recommended)
- Mozilla Firefox
- Microsoft Edge
- Safari

## Credits

Built with:
- PHP (Server-side logic)
- HTML5 (Structure)
- CSS3 (Styling)
- JavaScript (Interactivity)
- JSON (Data storage)

Icons by Font Awesome
Images by Unsplash

---

**Developer**: Mavangwa Andzani Singh
