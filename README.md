# 🧩 Join – Collaborative Kanban Board

A team-based Kanban board application built as part of a group project at the **Developer Akademie**.  
The goal was to design a functional task management tool with **HTML, CSS, and JavaScript**.

---

## 🚀 Overview

**Join** helps teams organize tasks visually and collaborate efficiently.  
Key features include task management, contacts handling, and drag & drop functionality.

---

## 🛠️ Tech Stack

- HTML5  
- CSS3  
- JavaScript (ES6)  
- Firebase (for user data and storage)  
- LocalStorage (for local session handling)  

---

## 📁 Project Structure
```yaml
join/
├── index.html
├── README.md
├── assets/
│ ├── fonts/
│ └── img/
├── includes/
├── overlays/
│ └── contacts/
├── pages/
├── scripts/
│ ├── add_task/
│ └── contacts/
├── styles/
│ └── contacts/
├── screenshots/
├── templates/
└── firebase/

```
Code kopieren

---

## 🔑 Firebase Setup

Since the original Firebase project was owned by Evgenij, create your **own Firebase project**:

1. Go to [Firebase Console](https://console.firebase.google.com/)  
2. Create a new project (e.g., `join-martin`)  
3. Add a web app and copy your Firebase config  
4. Create `firebase/firebaseConfig.js`:

```javascript
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT.firebaseapp.com",
  projectId: "YOUR_PROJECT",
  storageBucket: "YOUR_PROJECT.appspot.com",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID"
};

firebase.initializeApp(firebaseConfig);
Import this config in your scripts where needed.

👨‍💻 Team & Responsibilities
Name	Role	Focus Area
Martin Freimuth	Developer	Contacts module
Anne Sanewski	Developer	Task and board logic
Evgenij Liske	Developer	Sign-in and user handling

```
### 🖼️ Screenshots
# 🧩 Join – Collaborative Kanban Board

> A team-based Kanban board application for efficient task management and team collaboration

[![Live Demo](https://img.shields.io/badge/demo-live-success)](https://martin-frei.github.io/join/)


Developed as a collaborative group project at **Developer Akademie**, Join is a fully functional task management tool built with vanilla JavaScript, HTML5, and CSS3.

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Screenshots](#-screenshots)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [Firebase Setup](#-firebase-setup)
- [Team](#-team--responsibilities)
- [Future Enhancements](#-future-enhancements)
- [Contact](#-contact)

---

## 🚀 Overview

**Join** is a Kanban-style project management application that helps teams organize, track, and manage tasks visually. It features drag-and-drop functionality, user authentication, and a comprehensive contact management system.

### Key Highlights

✅ Intuitive drag-and-drop task management  
✅ User authentication with Firebase  
✅ Comprehensive contact management module  
✅ Responsive design for desktop, tablet, and mobile  
✅ Modular and maintainable code architecture  
✅ Real-time data synchronization

---

## ✨ Features

### Task Management
- Create, edit, and delete tasks
- Assign tasks to team members
- Set priorities (Low, Medium, Urgent)
- Add subtasks with progress tracking
- Drag-and-drop tasks between columns (To Do, In Progress, Awaiting Feedback, Done)

### Contact Management
- Add, edit, and delete contacts
- Store contact information (name, email, phone)
- Visual contact cards with color-coded avatars
- Search and filter functionality
- Detailed contact view

### User Authentication
- Secure login system
- User registration with validation
- Session management
- Guest access option

### UI/UX
- Clean, modern interface
- Responsive design (mobile-first approach)
- Smooth animations and transitions
- Toast notifications for user feedback
- Accessibility features

---

## 🖼️ Screenshots

### Kanban Board
![Kanban Board](screenshots/2025-11-10Screenshot_Join_KanBan_Board.png)

### Task Detail View
![Task Board](screenshots/2025-11-10Screenshot_Join_Task_Board.png)

### Contacts Module
![Contacts Module](screenshots/2025-11-10Screenshot_Join_Contacts.png)

---

## 🛠️ Tech Stack

### Frontend
- **HTML5** – Semantic markup and structure
- **CSS3** – Modern styling with Flexbox and Grid
- **JavaScript (ES6+)** – Modular architecture with async/await

### Backend & Database
- **Firebase Realtime Database** – User data and task storage
- **Firebase Authentication** – User management (optional)

### Storage
- **LocalStorage** – Session handling and temporary data

### Tools & Workflow
- **Git** – Version control
- **GitHub** – Code hosting and collaboration
- **VS Code** – Development environment

---

## 📁 Project Structure

```
join/
├── index.html                      # Landing/Login page
├── README.md                       # Project documentation
├── db_contacts.json               # Local contacts data backup
├── login_data.txt                 # Demo credentials
├── script.js                      # Main application logic
├── style.css                      # Global styles
│
├── assets/                        # Static resources
│   ├── fonts/                     # Custom web fonts (Inter)
│   └── img/                       # Icons and logos
│       ├── icons/                 # UI icons (buttons, forms, navigation)
│       └── logos/                 # Application logos
│
├── includes/                      # Reusable HTML components
│   ├── page_header.html
│   ├── page_navigation.html
│   └── add_task_form.html
│
├── overlays/                      # Modal dialogs
│   └── contacts/                  # Contact-specific overlays
│
├── pages/                         # Main application pages
│   ├── board.html                 # Kanban board view
│   ├── add_task.html             # Task creation page
│   ├── contacts_list.html        # Contacts overview
│   ├── summary.html              # Dashboard/summary
│   ├── help.html                 # Help documentation
│   ├── signup.html               # User registration
│   └── legal_notice.html         # Legal information
│
├── scripts/                       # JavaScript modules
│   ├── add_task/                 # Task creation logic
│   │   ├── add_tasks.js
│   │   ├── form_validation.js
│   │   └── form_selection/       # Form element handlers
│   │
│   ├── contacts/                 # Contact management (Martin's module)
│   │   ├── contacts.js           # Main controller
│   │   ├── contacts_firebase_api.js
│   │   ├── contacts_list_main.js
│   │   ├── contacts_validation.js
│   │   └── contacts_ui_helpers.js
│   │
│   ├── board_display_tasks.js    # Kanban board rendering
│   ├── task.js                   # Task operations
│   ├── login.js                  # Authentication logic
│   └── config.js                 # Application configuration
│
├── styles/                        # CSS modules
│   ├── contacts/                 # Contact-specific styles
│   ├── root.css                  # CSS variables and theme
│   ├── menu.css                  # Navigation styles
│   └── board.css                 # Kanban board styles
│
├── screenshots/                   # Application screenshots
└── templates/                     # HTML templates for dynamic content
```

---

## 🚀 Installation

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Git installed on your system
- Firebase account (for full functionality)

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/Martin-Frei/join.git
   cd join
   ```

2. **Open in browser**
   ```bash
   # Option 1: Direct file access
   open index.html
   
   # Option 2: Use a local server (recommended)
   python -m http.server 8000
   # Then open http://localhost:8000
   ```

3. **Login with demo credentials**
   - See `login_data.txt` for test accounts
   - Or create a new account via signup

### Using Your Own Firebase

For the full experience with persistent data storage, you'll need to set up Firebase:

---

## 🔥 Firebase Setup

The original Firebase project was managed by team member Evgenij. To use your own instance:

### Step 1: Create Firebase Project

1. Go to [Firebase Console](https://console.firebase.google.com/)
2. Click **"Add project"**
3. Name your project (e.g., `join-martin-2025`)
4. Follow the setup wizard (disable Google Analytics if not needed)

### Step 2: Add Web App

1. In your project, click the **web icon** (`</>`)
2. Register your app (name it "Join Web App")
3. Copy the Firebase configuration object

### Step 3: Configure Database

1. Go to **"Realtime Database"** in the left menu
2. Click **"Create Database"**
3. Choose a location (e.g., europe-west1)
4. Start in **test mode** (for development)

### Step 4: Add Configuration to Your Project

Create a new file `scripts/config.js` (if not exists) and add:

```javascript
// Firebase Configuration
const firebaseConfig = {
  apiKey: "AIzaSyXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
  authDomain: "your-project.firebaseapp.com",
  databaseURL: "https://your-project-default-rtdb.europe-west1.firebasedatabase.app",
  projectId: "your-project",
  storageBucket: "your-project.appspot.com",
  messagingSenderId: "123456789012",
  appId: "1:123456789012:web:abcdef123456"
};

// Initialize Firebase
firebase.initializeApp(firebaseConfig);
const database = firebase.database();

// Export for use in other modules
export { database, firebaseConfig };
```

### Step 5: Update HTML Files

Make sure your HTML files include the Firebase SDK:

```html
<!-- Add before closing </body> tag -->
<script src="https://www.gstatic.com/firebasejs/9.x.x/firebase-app-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/9.x.x/firebase-database-compat.js"></script>
<script src="scripts/config.js"></script>
```

### Security Rules (Optional)

For production, update your Firebase Database rules:

```json
{
  "rules": {
    "contacts": {
      "$uid": {
        ".read": "$uid === auth.uid",
        ".write": "$uid === auth.uid"
      }
    },
    "tasks": {
      "$uid": {
        ".read": "$uid === auth.uid",
        ".write": "$uid === auth.uid"
      }
    }
  }
}
```

---

## 👥 Team & Responsibilities

This project was developed collaboratively by three developers at Developer Akademie:

| Developer | GitHub | Primary Focus | Key Contributions |
|-----------|--------|---------------|-------------------|
| **Martin Freimuth** | [@Martin-Frei](https://github.com/Martin-Frei) | Contacts Module | Complete contact management system, Firebase integration, form validation, UI components |
| **Anne Sanewski** | - | Task & Board Logic | Kanban board implementation, drag-and-drop functionality, task CRUD operations |
| **Evgenij Liske** | - | Authentication | User login/signup system, session management, Firebase initial setup |

### Martin's Contributions (Contacts Module)

The entire contacts management system was developed by Martin Freimuth, including:

- **Backend Logic**: Firebase API integration, data persistence, CRUD operations
- **Frontend UI**: Contact list view, detail view, add/edit overlays
- **Form Handling**: Input validation, error handling, success notifications
- **User Experience**: Search functionality, responsive design, accessibility features

Files primarily developed by Martin:
- `scripts/contacts/*` (entire folder)
- `styles/contacts/*` (entire folder)
- `overlays/contacts/*` (all contact modals)
- `pages/contacts_list.html`

---

## 🔮 Future Enhancements

### Planned Features
- [ ] Backend migration to Django/Node.js for better scalability
- [ ] Real-time collaboration with WebSockets
- [ ] Dark mode and custom theme support
- [ ] Advanced task filtering and sorting
- [ ] Calendar integration for deadlines
- [ ] Email notifications for task assignments
- [ ] File attachments for tasks
- [ ] Activity log and audit trail
- [ ] Export functionality (CSV, PDF)
- [ ] Mobile app (React Native)

### Technical Improvements
- [ ] TypeScript migration for type safety
- [ ] Unit and integration tests
- [ ] CI/CD pipeline setup
- [ ] Performance optimization
- [ ] Offline mode with service workers
- [ ] Internationalization (i18n)

---

## 📝 License

This project was created as part of the Developer Akademie curriculum. Feel free to use it for learning purposes.

---

## 📬 Contact

**Martin Freimuth**  
Fullstack Developer | Python/Django | JavaScript/React

📍 Rosenheim, Bavaria, Germany  
📧 mat.frei@gmx.de  
🔗 [LinkedIn](https://www.linkedin.com/in/martin-freimuth)  
🔗 [GitHub](https://github.com/Martin-Frei)

---

## 🙏 Acknowledgments

- **Developer Akademie** – For the comprehensive web development program
- **Team Members** – Anne Sanewski and Evgenij Liske for their collaboration
- **Open Source Community** – For Firebase and various JavaScript libraries

---



**⭐ Star this repository if you find it helpful! ⭐**

Made with ❤️ by [Martin Freimuth](https://github.com/Martin-Frei)


**Kanban Board**  
![Kanban Board](screenshots/2025-11-10Screenshot_Join_KanBan_Board.png)

**Task Board**  
![Task Board](screenshots/2025-11-10Screenshot_Join_Task_Board.png)

**Contacts Module (by Martin Freimuth)**  
![Contacts Module](screenshots/2025-11-10Screenshot_Join_Contacts.png)
Images are responsive and scale down on smaller screens.

⚙️ Setup Instructions
Clone the repository:

bash
Code kopieren
git clone https://github.com/Martin-Frei/join.git
Open index.html in your browser

Replace Firebase credentials with your own (see Firebase section)

Enjoy your own version of Join

💡 Key Features
Drag & drop task organization

User login with Firebase

Contact management module (Martin's work)

Responsive design for all screen sizes

Modular JavaScript code structure

🧠 Future Improvements
Backend integration with Django or Node.js

Real-time database sync

Dark mode and theme customization

Authentication with tokens

📬 Contact
Martin Freimuth
📍 Rosenheim, Bavaria, Germany
📧 mat.frei@gmx.de
🔗 LinkedIn
🔗 GitHub