# Flask Official Docs Project

Welcome to the **Flask Official Docs Project** repository! This project is a comprehensive implementation of a Flask application, following the official Flask documentation. It serves as a reference and learning resource for building Flask applications.

## Repository Structure

```
flaskOfficialDocsProject
├── MANIFEST.in
├── __pycache__
│   └── setup.cpython-311.pyc
├── flaskr
│   ├── __init__.py
│   ├── __pycache__
│   │   ├── __init__.cpython-311.pyc
│   │   ├── auth.cpython-311.pyc
│   │   ├── blog.cpython-311.pyc
│   │   └── db.cpython-311.pyc
│   ├── auth.py
│   ├── blog.py
│   ├── db.py
│   ├── schema.sql
│   ├── static
│   │   └── style.css
│   └── templates
│       ├── auth
│       │   ├── login.html
│       │   └── register.html
│       ├── base.html
│       └── blog
│           ├── create.html
│           ├── index.html
│           └── update.html
├── flaskr.egg-info
│   ├── PKG-INFO
│   ├── SOURCES.txt
│   ├── dependency_links.txt
│   ├── not-zip-safe
│   ├── requires.txt
│   └── top_level.txt
├── instance
│   └── flaskr.sqlite
├── setup.cfg
├── setup.py
└── tests
    ├── __pycache__
    │   ├── conftest.cpython-311-pytest-8.2.1.pyc
    │   ├── test_auth.cpython-311-pytest-8.2.1.pyc
    │   ├── test_blog.cpython-311-pytest-8.2.1.pyc
    │   ├── test_db.cpython-311-pytest-8.2.1.pyc
    │   └── test_factory.cpython-311-pytest-8.2.1.pyc
    ├── conftest.py
    ├── data.sql
    ├── htmlcov
    │   ├── class_index.html
    │   ├── conftest_py.html
    │   ├── coverage_html_cb_6fb7b396.js
    │   ├── favicon_32_cb_58284776.png
    │   ├── function_index.html
    │   ├── index.html
    │   ├── keybd_closed_cb_ce680311.png
    │   ├── status.json
    │   ├── style_cb_8e611ae1.css
    │   ├── test_auth_py.html
    │   ├── test_blog_py.html
    │   ├── test_db_py.html
    │   ├── test_factory_py.html
    │   ├── z_f359065862a6cd71___init___py.html
    │   ├── z_f359065862a6cd71_auth_py.html
    │   ├── z_f359065862a6cd71_blog_py.html
    │   └── z_f359065862a6cd71_db_py.html
    ├── test_auth.py
    ├── test_blog.py
    ├── test_db.py
    └── test_factory.py
```

## Project Overview

This project includes the following components:

- **Application Code**: The main application logic is located in the `flaskr` directory, with separate modules for authentication (`auth.py`), blog functionality (`blog.py`), and database operations (`db.py`).
- **Templates**: HTML templates are stored in the `flaskr/templates` directory, organized into subdirectories for authentication (`auth`) and blog (`blog`).
- **Static Files**: Static files, such as CSS, are located in the `flaskr/static` directory.
- **Database**: The SQLite database file is stored in the `instance` directory.
- **Tests**: Unit tests for the application are located in the `tests` directory.

## Setup and Installation

1. **Clone the repository**:
   ```sh
   git clone https://github.com/yourusername/flaskOfficialDocsProject.git
   cd flaskOfficialDocsProject
   ```

2. **Create a virtual environment**:
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the dependencies**:
   ```sh
   pip install -e .
   ```

4. **Initialize the database**:
   ```sh
   flask --app flaskr init-db
   ```

5. **Run the application**:
   ```sh
   flask --app flaskr run
   ```

## Running Tests

To run the tests, execute the following command:
```sh
pytest
```

## Project Components

### `flaskr` Package

- **`__init__.py`**: Initializes the Flask application and registers the blueprints.
- **`auth.py`**: Handles user authentication, including registration and login.
- **`blog.py`**: Manages the blog functionality, including creating, updating, and displaying posts.
- **`db.py`**: Manages database connections and operations.
- **`schema.sql`**: Contains the SQL schema for initializing the database.

### Templates

- **`base.html`**: The base template used by other templates.
- **Authentication Templates**:
  - `login.html`
  - `register.html`
- **Blog Templates**:
  - `create.html`
  - `index.html`
  - `update.html`

### Tests

- **`conftest.py`**: Configuration for pytest.
- **`test_auth.py`**: Tests for the authentication module.
- **`test_blog.py`**: Tests for the blog module.
- **`test_db.py`**: Tests for the database module.
- **`test_factory.py`**: Tests for the application factory.

## Resources

For more information, refer to the official [Flask documentation](https://flask.palletsprojects.com/en/3.0.x/).

## Contribution

Feel free to open issues or submit pull requests for improvements or bug fixes. Contributions are welcome!

---

Thank you for checking out this project. Happy coding!
