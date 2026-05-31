# Todo List Application

A web-based Todo List application built with Django, featuring user authentication and task management.

## Features

- **User Authentication**: Sign up and log in securely
- **Task Management**: Create, read, update, and delete tasks
- **Responsive Design**: Mobile-friendly interface
- **User-Specific Tasks**: Each user can manage their own tasks
- **Persistent Storage**: Tasks are saved to a database

## Technologies Used

- **Backend**: Django
- **Database**: SQLite (default)
- **Frontend**: HTML, CSS, JavaScript
- **Admin Panel**: Django Admin

## Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd TodoList
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run migrations**
   ```bash
   python manage.py migrate
   ```

5. **Create a superuser (optional)**
   ```bash
   python manage.py createsuperuser
   ```

6. **Start the development server**
   ```bash
   python manage.py runserver
   ```

7. **Access the application**
   - Main app: `http://localhost:8000/`
   - Admin panel: `http://localhost:8000/admin/`

## Project Structure

```
TodoList/
├── Todo_list/              # Main Django app
│   ├── models.py          # Database models
│   ├── views.py           # View logic
│   ├── urls.py            # URL routing
│   ├── templates/         # HTML templates
│   │   ├── login.html
│   │   ├── signup.html
│   │   ├── todo.html
│   │   └── edit_task.html
│   └── static/            # Static files (CSS, JS)
├── manage.py              # Django management script
├── requirements.txt       # Python dependencies
├── Procfile              # Heroku deployment configuration
├── runtime.txt           # Python version for deployment
└── db.sqlite3            # SQLite database
```

## Usage

1. **Sign Up**: Create a new account by providing a username and password
2. **Log In**: Log in with your credentials
3. **Create Tasks**: Add new tasks from the main dashboard
4. **Edit Tasks**: Modify existing tasks
5. **Delete Tasks**: Remove tasks you no longer need
6. **Log Out**: Securely log out of your account

## Deployment

This application is configured for deployment on Heroku. Make sure to:
- Update `ALLOWED_HOSTS` in `settings.py` for your domain
- Set environment variables for production
- Use a production database (PostgreSQL recommended)

## Requirements

See `requirements.txt` for all dependencies.

## License

This project is open source and available under the MIT License.

## Contributing

Contributions are welcome! Please feel free to submit a pull request.

## Support

For issues or questions, please open an issue in the repository.
