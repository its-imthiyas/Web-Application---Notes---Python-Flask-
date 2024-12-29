# Flask Web App: Authentication & Notes Management

This repository contains the source code for a Flask-based web application designed for secure user authentication and efficient notes management. The application demonstrates full-stack development with robust backend security and user-friendly features.

## Features

### Authentication
- **User Registration**: 
  - Email validation (must follow proper email format).
  - Password requirements (minimum character length).
  - Name validation.
  - Prevents duplicate registrations by checking if the email already exists in the database.
- **Secure Login**: User sessions are managed securely using `Flask-Login`.
- **Session Management**: Protects routes to ensure only authenticated users can access specific pages.

### Notes Management
- **Create, Read, Update, and Delete (CRUD)** operations for managing user notes.
- Notes are associated with individual users to ensure privacy and security.
- Responsive and intuitive interface for seamless notes management.

## Technologies Used

- **Backend**: Flask, Flask-Login, SQLAlchemy
- **Database**: SQLAlchemy ORM for seamless database integration
- **Frontend**: HTML, CSS, JavaScript (if applicable for dynamic features)

## Setup and Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/flask-web-app-auth-notes.git
   cd flask-web-app-auth-notes
   ```

2. **Create a Virtual Environment**:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up the Database**:
   Initialize the database with SQLAlchemy (details provided in the app). Example:
   ```bash
   flask db init
   flask db migrate -m "Initial migration."
   flask db upgrade
   ```

5. **Run the Application**:
   ```bash
   flask run
   ```
   The application will be available at `http://127.0.0.1:5000/`.

## Usage

1. **Registration Rules**:
   - Use a valid email format.
   - Password must meet the minimum character length.
   - Ensure the email is not already registered.

2. **Logging In**:
   - Use the registered email and password to log in.
   - Access to notes management features is restricted to logged-in users.

3. **Notes Management**:
   - Create, edit, and delete personal notes via a user-friendly interface.

## Image Representation
Here is a image showing the application in action:
[!(https://github.com/its-imthiyas/Web-Application-Notes-Authentication--Python-Flask/blob/main/WebPage%20Screenshot.jpg)]

## Future Improvements
- Add multi-language support.
- Implement advanced search and filtering for notes.
- Introduce rich-text editing for notes.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
