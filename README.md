📝 Lost and Found Management System

C# Desktop Application | Visual Studio Community | SQL Database (if using)

A desktop application built with C# in Visual Studio Community to manage lost and found items in a university. Features include Admin and Student authentication, adding/viewing lost & found items, item matching, and tracking returned items.

🎓 Project Information

Course: Software Engineering Fundamentals (SEF)
Semester: 3rd Semester
Author: Fahad Munir
Institution: National Textile University (NTU)

🌟 Features

Authentication & Authorization
✅ Admin and Student login with username and password
✅ Student accounts created by Admin with Student ID
✅ Student dashboard displays username and personalized view

Student Features
✅ Add Lost Item – Enter item name, description, location, date (auto-filled), contact info, and upload image
✅ Add Found Item – Similar form to add found items
✅ View My Matches – Check if any lost/found items match their submissions
✅ View Returned – Track if matched items have been returned to the owner
✅ Logout – Securely log out from dashboard

Admin Features
✅ Add Student – Register new students with username, password, and Student ID
✅ View Lost Items – See all lost items with details and images
✅ View Found Items – See all found items with details and images
✅ Manual Match – Approve matches between lost and found items
✅ Mark as Returned – Update items that have been returned to the owner
✅ Dashboard Stats – Display total lost items, found items, and matched items
✅ Logout – Securely log out from dashboard

🛠️ Tech Stack

Backend & Frontend

C# (Desktop Application)

Visual Studio Community IDE

Windows Forms / WPF (for GUI)

SQL Database (or local storage)

Features Implemented Using

Forms for inputting lost/found items

Dashboard interfaces for Admin and Students

Image uploading functionality

Auto-generated date entries

Item matching and status tracking

📁 Project Structure
LostAndFoundManagementSystem/
│
├── LoginForm.cs                # Login interface for Admin & Students
├── StudentDashboard.cs         # Student dashboard interface
├── AdminDashboard.cs           # Admin dashboard interface
├── AddLostItemForm.cs          # Form to add lost items
├── AddFoundItemForm.cs         # Form to add found items
├── ViewMatchesForm.cs          # Student view matches form
├── AddStudentForm.cs           # Admin add student form
├── ViewLostItemsForm.cs        # Admin view lost items
├── ViewFoundItemsForm.cs       # Admin view found items
├── ManualMatchForm.cs          # Admin manual match form
├── Database/                   # Database files or connection scripts
│   └── DatabaseConnection.cs
└── Images/                     # Folder for uploaded images

🚀 Installation & Setup

Prerequisites

Windows OS

Visual Studio Community installed

.NET Framework (4.7 or higher)

SQL Server or local database setup (if used)

Steps

Clone the Repository:

git clone https://github.com/yourusername/LostAndFoundManagementSystem.git
cd LostAndFoundManagementSystem


Open in Visual Studio Community.

Build Solution (Ctrl+Shift+B) to restore dependencies.

Run the application (F5).

Use Admin credentials to add students and test functionality.

📋 Database Schema (Example)

Student Table

StudentID   INT (Primary Key)
Username    VARCHAR
Password    VARCHAR
Name        VARCHAR


LostItem Table

ItemID      INT (Primary Key)
ItemName    VARCHAR
Description TEXT
Location    VARCHAR
Date        DATETIME
StudentID   INT (Foreign Key)
Contact     VARCHAR
ImagePath   VARCHAR


FoundItem Table

ItemID      INT (Primary Key)
ItemName    VARCHAR
Description TEXT
Location    VARCHAR
Date        DATETIME
StudentID   INT (Foreign Key)
Contact     VARCHAR
ImagePath   VARCHAR


Matches Table

MatchID     INT (Primary Key)
LostItemID  INT (Foreign Key)
FoundItemID INT (Foreign Key)
MatchDate   DATETIME
Returned    BIT

🔒 Security & Validation

Passwords stored securely (hashed if implemented)

Only Admin can add student accounts

Students can only view/edit their own items

Input validation on all forms

File upload restricted to image types

📝 Future Enhancements

Email notifications when items are matched

Barcode/QR code for lost/found items

Mobile app version

Advanced search and filter options

Admin analytics dashboard

🤝 Contributing

This is a semester project, but suggestions and improvements are welcome!

Fork the repository

Create a feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request

📄 License

This project is licensed under the ISC License.

👥 Author

Fahad Munir – Lead Developer
Institution: National Textile University (NTU)
Course: Software Engineering Fundamentals (SEF)
Semester: 3rd Semester

🙏 Acknowledgments

Visual Studio Community IDE

Microsoft Windows Forms / WPF Documentation

C# Programming Resources

SQL Server / Database Management Resources

📞 Support

For questions or issues:

GitHub Issues: Create an issue

Email: Contact through GitHub profile

📸 Screenshots

Login Form – Admin & Student login interface

Student Dashboard – Add lost/found items, view matches, logout

Admin Dashboard – Dashboard stats, add student, view items, manual match

Add/Update Forms – Input forms with image upload and auto date
