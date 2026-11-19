# LibraryHub — Online Library Management System

A web-based **Online Library Management System** prototype developed as a group project for **Internet Programming I (INSY3061)** at Wollo University, Kombolcha Institute of Technology.

LibraryHub is intended to make it easier for library visitors to discover books and for registered members and librarians to manage book requests and borrowing activities through one responsive web interface.

> **Project status:** In development. The homepage HTML structure has been created. CSS styling, the remaining page interfaces, and JavaScript functionality are being developed.

## Project Objectives

- Provide a simple interface for browsing and searching the library catalog.
- Allow visitors to register and sign in as library members.
- Allow members to submit book-borrowing requests and track their status.
- Allow librarians/administrators to manage books and review borrowing requests.
- Practice semantic HTML, responsive CSS, JavaScript, collaboration, and Git/GitHub version control.

## User Roles

### 1. Guest

A visitor who has not signed in can:
- View the homepage and library information.
- Browse the book catalog.
- Search and filter books.
- View book details and availability.
- Navigate to the registration or login page.

Guests cannot submit borrowing requests.

### 2. Member

A registered member can:
- Register and sign in.
- Browse, search, and view books.
- Submit a borrowing request for an available book.
- View request status (pending, approved, rejected, or cancelled).
- View currently borrowed books, due dates, and borrowing history.
- Manage permitted profile information and sign out.

### 3. Administrator / Librarian

An administrator can:
- Sign in to the administration area.
- View library summary information.
- Add, edit, view, and remove book records.
- Manage book categories.
- Review and approve or reject member requests.
- Record when an approved book is issued and when it is returned.
- View member records and submitted feedback.

## Main Borrowing Workflow

1. A guest browses the catalog and opens a book's details.
2. To request a book, the visitor registers or signs in as a member.
3. The member submits a borrowing request.
4. The request is initially marked **Pending**.
5. The librarian reviews the request and approves or rejects it.
6. An approved request is reserved for the member. When the member collects the book, the librarian records it as **Borrowed** and sets a due date.
7. When the book is returned, the librarian records the return and the available-copy count is updated.

## Planned Features

- Responsive homepage and navigation.
- Book catalog with search and category/availability filters.
- Book details view.
- Member registration and login interfaces with form validation.
- Member dashboard for requests, borrowed books, and history.
- Administrator dashboard for book, category, member, and request management.
- Borrowing and return status updates.
- Contact/help form.

Features are being implemented in stages. The list above describes the intended project scope and does not imply that every feature is already complete.

## Technology Stack

| Technology / Tool | Purpose |
|---|---|
| HTML5 | Page structure and semantic content |
| CSS3 | Styling, layout, and responsive design |
| JavaScript | Client-side interactions, validation, search, and prototype data handling |
| Figma | UI/UX planning and wireframes |
| Visual Studio Code | Development environment |
| Git | Local version control |
| GitHub | Shared repository and team collaboration |

The agreed initial implementation is a **front-end prototype**. Structured sample data and browser `localStorage` may be used for demonstration. This version does not provide production-grade server-side authentication, centralized multi-device data storage, or backend security.

## Project Structure

```text
library_system/
├── assets/                 # Additional assets (e.g. icons or fonts)
├── css/
│   └── style.css           # Shared site styles
├── images/                 # Book covers, logos, and other images
├── js/
│   ├── data.js             # Prototype data (books, categories, etc.)
│   └── main.js             # Shared JavaScript functionality
├── pages/
│   ├── admin-dashboard.html
│   ├── catalog.html
│   ├── contact.html
│   ├── login.html
│   └── user-dashboard.html
└── index.html              # Homepage / application entry point
```

The structure may be extended as the project develops (for example, with a registration page or a separate book-details page).

## Getting Started

### Requirements

- A modern web browser.
- Visual Studio Code (recommended for development).
- The **Live Server** extension for VS Code (recommended for local preview).
- Git, if you plan to contribute to the repository.

### Run locally

1. Clone the repository:

   ```bash
   git clone <repository-url>
   ```

2. Open the project folder in Visual Studio Code:

   ```bash
   cd library_system
   code .
   ```

3. Open `index.html` with the VS Code **Live Server** extension, or open the file directly in a browser for basic static-page preview.

4. As additional pages and JavaScript functionality are completed, test the relevant pages and interactions in the browser.

## Development Workflow

The project is developed in small, reviewable stages:

1. Requirements and system architecture.
2. Figma wireframes and shared UI components.
3. HTML page structure.
4. CSS styling and responsive layouts.
5. JavaScript interactions and prototype data handling.
6. Integration of member and administrator workflows.
7. Testing, bug fixing, documentation, and demonstration.

### Git contribution guidelines

- Pull the latest changes before starting work.
- Work on a focused feature or task at a time.
- Use clear commit messages, for example:

  ```text
  feat(home): add hero and navigation structure
  style(home): implement responsive homepage layout
  feat(catalog): add book search and category filters
  fix(auth): validate registration form inputs
  ```

- Avoid committing generated files, personal information, passwords, API keys, or other secrets.
- Coordinate changes to shared files such as `css/style.css` and `js/main.js` with the group to reduce merge conflicts.

## Testing Checklist

Before a feature is considered complete, check that:

- Navigation links open the correct pages.
- Forms have labels and appropriate input validation.
- Search and filtering return the expected books.
- Request status changes follow the agreed borrowing workflow.
- Layouts work on desktop and mobile screen sizes.
- Interactive controls can be used with a keyboard where applicable.
- The major pages work in at least two browsers where possible.

## Team Members

Group members          ID
1,Aymen Nuru.......... 0125/17
2,Tilahun kindie...... 1976/17
3,Mubark Enders......1701/17
4,Netsant Andargachew...1769/17
5,Siham Seid.................... 1885/17
6,Meskerm Demssie ... 1650/17

## Course Information

- **Course:** Internet Programming I (INSY3061)
- **Institution:** Wollo University
- **Campus/Institute:** Kombolcha Institute of Technology
- **Department:** Information Systems
- **Project:** Group Web Project — Online Library Management System

## Acknowledgment

This project is an academic group project. All group members are expected to understand the parts they contribute to, participate in integration and testing, and acknowledge any external libraries, tutorials, or resources used.
