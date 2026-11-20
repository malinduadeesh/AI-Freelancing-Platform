# AI Projects & Services Freelancing Platform

**Module:** PUSL2019 – Information Management & Retrieval  

## 1. Project Overview

The **AI Projects & Services Freelancing Platform** is a web-based freelancing marketplace designed to connect clients and organisations with freelancers who specialise in Artificial Intelligence (AI)-related skills and services.

The platform allows clients to post AI-related projects, define project requirements, review freelancer proposals, assign projects and monitor progress.

Freelancers can register, create professional profiles, showcase their AI skills and services, browse available projects and submit proposals.

The platform also supports assignment management, payment records, two-way reviews, administrative management and reporting.

This project focuses on implementing a relational database system integrated with a functional web application.

**Note:** The platform manages AI-related projects and services. Developing or training an AI model is not required. Real payment gateway integration is outside the current scope.

## 2. Project Objectives

The main objectives of this project are:

1. Develop a database-driven freelancing platform for AI-related projects and services.
2. Allow freelancers and clients to register and manage their profiles.
3. Enable clients to publish projects and specify AI skill requirements.
4. Allow freelancers to submit proposals for available projects.
5. Support proposal selection and freelancer assignment management.
6. Track project and assignment progress.
7. Maintain payment records and reviews.
8. Provide administrative functions and management reports.
9. Demonstrate relational database design, normalization and advanced SQL operations.
10. Integrate the database with a functional web interface.

## 3. Main System Features

### Freelancer Features

- Freelancer registration and login
- Profile creation and management
- AI skills and services management
- Browse available projects
- Submit and manage proposals
- View assigned work and update authorized progress
- View payment records
- Submit reviews after completed assignments

### Client Features

- Client registration and login
- Client and organisation profile management
- Create and manage projects
- Define project requirements and required AI skills
- Review submitted proposals
- Accept multiple suitable proposals
- Create and monitor assignments
- Record payment information
- Submit reviews after completed assignments

### Administrator Features

- Administrator login
- Manage freelancer and client accounts
- Manage AI skills and service categories
- Monitor platform projects and proposals
- Maintain platform information

### Manager Features

- Manager login
- View project summaries
- View freelancer and client statistics
- Monitor proposals and assignments
- View payment and activity reports

## 4. Technologies Used

The project uses the following technologies:

| Technology | Purpose | Official Website |
|---|---|---|
| HTML5 | Structure of web pages | https://developer.mozilla.org/en-US/docs/Web/HTML |
| CSS3 | Styling and page design | https://developer.mozilla.org/en-US/docs/Web/CSS |
| JavaScript | Client-side functionality and validation | https://developer.mozilla.org/en-US/docs/Web/JavaScript |
| Bootstrap 5 | Responsive user interface | https://getbootstrap.com/ |
| PHP | Backend development and server-side processing | https://www.php.net/ |
| MySQL-compatible SQL database | Database storage and management | https://dev.mysql.com/downloads/ |
| Apache | Local web server | https://httpd.apache.org/ |
| Git | Version control | https://git-scm.com/ |
| GitHub | Repository hosting and collaboration | https://github.com/ |

**Technology note:** XAMPP provides Apache, PHP, MariaDB (MySQL-compatible) and phpMyAdmin for local development. Separate installation of these components is not necessary when using XAMPP.

## 5. Required Software and Download Links

All team members should install the following software to set up the project locally.

| Software | Purpose | Download Link |
|---|---|---|
| Visual Studio Code | Code editor | https://code.visualstudio.com/download |
| XAMPP | Local Apache, PHP and database environment | https://www.apachefriends.org/download.html |
| Git | Version control | https://git-scm.com/downloads |
| GitHub Desktop | Manage repositories, branches, commits and pull requests | https://desktop.github.com/download/ |
| diagrams.net (draw.io) | ERD creation and editing | https://app.diagrams.net/ |
| MySQL Workbench (Optional) | SQL development and database modeling | https://dev.mysql.com/downloads/workbench/ |

### Additional Technology Resources

**Bootstrap 5**

Official website: https://getbootstrap.com/

Bootstrap can be included using a CDN or downloaded directly.

**PHP**

Official downloads: https://www.php.net/downloads.php

PHP is already included in XAMPP.

**MySQL**

Official downloads: https://dev.mysql.com/downloads/

The project uses the MySQL-compatible MariaDB database included with XAMPP.

**HTML, CSS and JavaScript**

These technologies do not require separate installation. They are written in VS Code and executed through the browser.

## 6. Project Folder Structure

The following folder structure is used in the GitHub repository:

```text
AI-Freelancing-Platform/
│
├── admin/
│
├── auth/
│
├── client/
│
├── database/
│
├── docs/
│
├── freelancer/
│
├── includes/
│
├── public/
│   └── index.php
│
├── tests/
│
├── .gitattributes
│
└── README.md
```

### Folder Descriptions

| Folder | Purpose |
|---|---|
| admin | Administrator and management reporting features |
| auth | Registration, login, logout and authentication |
| client | Client dashboard, project posting and proposal management |
| database | SQL database schema, sample data and SQL objects |
| docs | ERD, relational mapping, normalization and project documentation |
| freelancer | Freelancer dashboard, profiles, skills and services |
| includes | Shared PHP files, database connection and helper functions |
| public | Main website entry point and frontend assets |
| tests | Testing documentation, test cases and evidence |

Additional PHP, CSS, JavaScript and SQL files will be added as development progresses.

## 7. GitHub Repository

**Repository Name:** AI-Freelancing-Platform

**GitHub Repository Link:**

https://github.com/malinduaadeesh/AI-Freelancing-Platform

All team members will collaborate using this shared repository.

Each member should work on their assigned branch and submit completed changes through Pull Requests.

## 8. Local Development Setup

Follow these steps to run the project locally.

### Step 1: Install the Required Software

Install:

1. Visual Studio Code
2. XAMPP
3. Git
4. GitHub Desktop

Use the official download links provided in Section 5.

### Step 2: Clone the GitHub Repository

1. Open GitHub Desktop.
2. Sign in to your GitHub account.
3. Select **File → Clone Repository**.
4. Select the `AI-Freelancing-Platform` repository or paste its URL.
5. Choose a local folder.
6. Click **Clone**.
7. Open the repository in Visual Studio Code.

### Step 3: Start XAMPP

1. Open XAMPP Control Panel.
2. Start **Apache**.
3. Start **MySQL**.
4. Ensure both services are running.

### Step 4: Make the Project Accessible Through XAMPP

The project must be accessible through the XAMPP `htdocs` directory.

For a simple setup, place the cloned project folder inside:

`C:\xampp\htdocs\`

Alternatively, configure a directory junction linking the cloned repository to `htdocs`.

Ensure the accessible folder is named:

`AI-Freelancing-Platform`

### Step 5: Create the Local Database

1. Open a web browser.
2. Navigate to http://localhost/phpmyadmin/
3. Select **New**.
4. Create a database named:

   `ai_freelancing_db`

5. Select the collation:

   `utf8mb4_unicode_ci`

6. Click **Create**.

When the SQL implementation is completed, import the database schema and sample data from the `database/` folder.

Each team member must configure their own local database.

### Step 6: Run the Project

Open the following URL:

http://localhost/AI-Freelancing-Platform/public/index.php

During the initial setup stage, the page displays:

`AI Freelancing Platform - PHP is working!`

This confirms that PHP and Apache are functioning correctly.

The complete application will become available as development progresses.

## 9. Database Design

The platform uses a relational database designed using an Entity Relationship Diagram (ERD).

The database design includes 15 tables:

1. Freelancer
2. Client
3. Admin
4. Manager
5. AISkill
6. AIService
7. FreelancerSkill
8. FreelancerService
9. Project
10. ProjectSkill
11. ProjectRequirement
12. Proposal
13. Assignment
14. Payment
15. Review

### Database Documentation

The `docs/` folder will contain:

- Final Entity Relationship Diagram
- Requirements and assumptions
- Relational mapping
- Normalization up to Third Normal Form (3NF)
- Data dictionary
- Database design documentation

The `database/` folder will contain:

- Database schema SQL file
- Sample data SQL file
- Triggers
- User-defined functions
- Views
- Stored procedures

## 10. Important Business Rules

The system follows the approved project assumptions.

- Freelancer, Client, Admin and Manager have separate account tables.
- A client can create multiple projects.
- A freelancer can submit proposals to multiple projects.
- A freelancer can have only one active proposal per project, according to the agreed active-status rule.
- A client can accept multiple proposals for one project.
- One accepted proposal can produce multiple assignments.
- Multiple freelancers can work on the same project.
- A project can require multiple AI skills.
- Payments are recorded against assignments.
- Each assignment can have a maximum of one payment record.
- Clients and freelancers can review each other after assignment completion.
- Each reviewer role can submit only one review per assignment.
- A project can be marked Completed only when it has at least one assignment and all its assignments are completed.

### Project Statuses

- Open
- Assigned
- In Progress
- Completed
- Cancelled

### Proposal Statuses

- Pending
- Accepted
- Rejected
- Withdrawn

## 11. Team Responsibilities

| Member | Role | Responsibilities |
|---|---|---|
| Member 1 | Team Leader & Database Designer | Requirements, assumptions, ERD, relational mapping, normalization and coordination |
| Member 2 | SQL Database Developer | Database creation, tables, sample data, triggers, functions, views and stored procedures |
| Member 3 | Frontend Developer | Website interface, responsive layouts, dashboards and forms |
| Member 4 | Backend Developer & Integration Lead | PHP backend, authentication, database connectivity and application workflows |
| Member 5 | QA, Reporting & Admin/Analytics | Testing, bug tracking, management reports and report coordination |

## 12. GitHub Collaboration Workflow

To avoid conflicts, all team members must follow the agreed GitHub workflow.

### Working on the Project

1. Clone the shared GitHub repository.
2. Create or switch to your assigned branch.
3. Pull the latest changes before starting work.
4. Work on your assigned files.
5. Save and test your changes.
6. Commit with a meaningful commit message.
7. Push your branch to GitHub.
8. Create a Pull Request targeting `main`.
9. Review and merge approved changes.

### Important Guidelines

- Do not directly overwrite another member's work.
- Communicate before modifying shared files.
- Do not upload passwords or confidential information.
- Keep database credentials out of public commits.
- Use meaningful commit messages.
- Test changes before merging.
- Keep the main branch stable.

## 13. Security Considerations

The project should follow basic web application security practices.

- Store passwords using secure password hashing.
- Use prepared SQL statements to prevent SQL injection.
- Validate inputs on the server side.
- Restrict pages and actions based on user roles.
- Prevent unauthorized access to client and freelancer information.
- Avoid exposing sensitive database configuration details.
- Do not commit real passwords, credentials or private user data to GitHub.

## 14. Testing

The project will be tested to verify the main workflows.

Testing will cover:

- User registration and login
- Role-based access
- Freelancer profile management
- Project creation and management
- Proposal submission and selection
- Assignment creation and progress tracking
- Payment record management
- Review submission
- Database constraints
- SQL triggers, functions, views and stored procedures
- Admin and manager reporting

Testing results and evidence will be maintained in the `tests/` folder.

## 15. Project Deliverables

The final coursework submission will include:

1. Complete project report
2. ER/EER diagram and database design documentation
3. Relational mapping and normalization to 3NF
4. Data dictionary
5. SQL database implementation
6. Sample database records
7. Required triggers, functions, views and stored procedures
8. Functional web application
9. Testing and evaluation evidence
10. Public GitHub repository link
11. Recorded group presentation
12. Required Generative AI declaration

## 16. Current Development Status

**Project Status:** In Development

Completed initial activities:

- GitHub repository created
- Project folder structure established
- VS Code environment configured
- XAMPP local environment tested
- PHP execution verified
- Initial local database created
- ERD Version 5 finalized
- Relational mapping drafted

Upcoming activities:

- Complete normalization to 3NF
- Prepare and verify the data dictionary
- Implement SQL database tables and constraints
- Add sample data and advanced SQL objects
- Develop frontend and backend features
- Integrate the application
- Perform testing and complete documentation

## 18. How a New User Can Open the Website

A new team member must follow these steps to access the AI Freelancing Platform on their local computer.

### Step 1: Install the Required Software

Install the following:

* Visual Studio Code
* XAMPP
* Git
* GitHub Desktop

Refer to Section 5 for the official download links.

### Step 2: Download the Project

1. Open GitHub Desktop.
2. Sign in to your GitHub account.
3. Select **File → Clone Repository**.
4. Select the `AI-Freelancing-Platform` repository.
5. Choose a location on your computer.
6. Click **Clone**.

### Step 3: Set Up the Project Folder

1. Locate the cloned project folder.
2. Copy or make the project accessible inside the XAMPP `htdocs` folder.
3. The folder path should be:

   `C:\xampp\htdocs\AI-Freelancing-Platform`

### Step 4: Start XAMPP

1. Open XAMPP Control Panel.
2. Start Apache.
3. Start MySQL.
4. Ensure both services are running.

### Step 5: Set Up the Database

1. Open Chrome or another web browser.
2. Visit http://localhost/phpmyadmin/
3. Create a database named `ai_freelancing_db`.
4. Import the database SQL file from the project's `database/` folder once it is available.
5. Configure the local database connection using the project's database configuration instructions.

### Step 6: Open the Website

1. Open your web browser.

2. Enter the following address:

   `http://localhost/AI-Freelancing-Platform/public/index.php`

3. Press Enter.

4. The website should open in your browser.

### Important Notes

* Apache and MySQL must be running whenever the locally hosted website is accessed.
* Each team member must configure their own local development environment and database.
* The website is accessed locally through XAMPP; `localhost` does not automatically make it accessible to other computers.
* The complete application will become available as the development and integration work progresses.
