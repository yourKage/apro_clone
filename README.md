# Apro Test System

Apro Test System is a Django-based application that allows users to register, log in, and view their test results. The application uses a custom SQLite database for user authentication and stores user details.

## Features

- User registration with phone number
- User login with phone number and password
- Dashboard displaying user details
- View test categories and results
- Admin features for managing users and tests
- Teacher features for creating and managing tests

## Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/yourusername/apro-test-system.git
    cd apro-test-system
    ```

2. Create a virtual environment and activate it:

    ```sh
    python -m venv .venv
    .venv\Scripts\activate  # On Windows
    source .venv/bin/activate  # On macOS/Linux
    ```

3. Install the required dependencies:

    ```sh
    pip install -r requirements.txt
    ```

4. Apply the database migrations:

    ```sh
    python manage.py migrate
    ```

5. Create a superuser:

    ```sh
    python manage.py createsuperuser
    ```

6. Run the development server:

    ```sh
    python manage.py runserver
    ```

## Usage

### Registering a User

1. Start the bot by running the `bot.py` script:

    ```sh
    python test_system/bot.py
    ```

2. Open your Telegram app and start a chat with your bot.
3. Send the `/start` command to the bot.
4. Follow the instructions to send your contact information and confirm registration.
5. The bot will generate a unique password and send it to you.

### Logging In

1. Open your web browser and navigate to `http://localhost:8000/login/`.
2. Enter your phone number and password provided by the bot.
3. Click the "Login" button.

### Viewing the Dashboard

1. After logging in, you will be redirected to the dashboard.
2. The dashboard will display a personalized greeting with your username.
3. You can view your test results and test categories from the dashboard.

### Admin Features

1. Log in as the superuser created during installation.
2. Navigate to the Django admin interface at `http://localhost:8000/admin/`.
3. Manage users, tests, categories, and other models from the admin interface.

### Teacher Features

1. Log in as a teacher.
2. Navigate to the teacher dashboard.
3. Create and manage tests, questions, and choices.
4. View test results for students.
 
## Contributing

Contributions are welcome! Please open an issue or submit a pull request if you have any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
