# Contactual — Contact Book Manager (POOSD Small Project)

Contactual is a lightweight contact book manager that centralizes all your contacts into a simple web interface. Users can register/login, add contacts, edit or delete them, and quickly search through saved entries. Contacts are stored per-user, so each account only sees their own contact list.

## Features
- Login / Register landing page
- Users cannot log in without a registered account
- Add contacts
- Edit / delete contacts
- Search contacts
- Contacts are stored per unique user account

## Tech Stack
- **Frontend:** HTML, JavaScript, CSS
- **Backend/API:** PHP (REST-style API endpoints)
- **Database:** MySQL
- **Hosting:** DigitalOcean

## Project Structure
```
poosd_small_project/
├── api/
│   ├── loginContact.php
│   ├── registerContact.php
│   ├── searchContact.php
│   ├── addContact.php
│   ├── deleteContract.php
│   └── editContact.php
│
├── css/
│   ├── start_style.css
│   └── styles.css
│
├── images/
│   └── contactual-logo.png
│
├── js/
│   ├── api.js
│   ├── auth.js
│   ├── config.js
│   ├── contacts.js
│   └── md5.js
│
├── .gitignore
├── README.md
├── contact.html
└── index.html
```

## How to Use (Hosted)
No local commands are required to use the app, simply open the deployed website URL in your browser.

1. Open the site
2. Register an account
3. Log in
4. Add, edit, delete, or search contacts

## Local Setup (Building/Running From Source)

### Prerequisites
- A web server capable of running PHP (e.g., Apache or Nginx)
- PHP installed (version depends on your environment/server)
- MySQL database
- Ability to host the static frontend files (`index.html`, `contact.html`, plus `css/`, `js/`, `images/`)

### Configuration
The API requires database credentials via a `config.php` file (not committed to the repo). Create a `config.php` with your own database credentials in the location expected by the API code.

> Note: The repo references 'config.php' for DB credentials, so you must provide your own before the API endpoints can connect to MySQL.

### Running Locally
1. Place the project in your PHP server’s web root (or configure a vhost/site to point at it).
2. Ensure MySQL is running and your schema/tables are created (per your project’s DB setup).
3. Add your `config.php` file with valid credentials.
4. Open `index.html` in the browser via your local server URL (not as a raw file path).

## API Endpoints
API endpoints live in the `api/` directory:
- `loginContact.php`
- `registerContact.php`
- `searchContact.php`
- `addContact.php`
- `deleteContract.php`
- `editContact.php`

## Testing
API endpoints were tested using **SwaggerHub Studio**.

## Contributors
- **Anna Russell** — Project Manager  
- **Horacio Sierra Perez** — Frontend  
- **Karina Ann** — Frontend  
- **Sydney Lalah** — Frontend  
- **Joshua Pache** — API  
- **Zakaria Khan** — API  
- **Annie Tsai** — Database  

## License
This project is licensed under the **MIT License**. See `LICENSE` for details.
