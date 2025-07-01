# Little Lemon Booking API

Booking system for the Little Lemon restaurant, built with Django and MySQL integration.

## 📋 Description

This project implements a complete booking system for the Little Lemon restaurant, allowing customers to make online reservations and view all existing bookings. The system uses Django as the web framework and MySQL as the database.

## 🚀 Technologies Used

- **Django 4.2.23** - Python web framework
- **MySQL** - Relational database
- **Python 3.9** - Programming language
- **Pipenv** - Dependency manager and virtual environment
- **HTML/CSS** - Frontend and styling
- **JavaScript** - Frontend interactivity

## 📦 Installation

### Prerequisites

- Python 3.9+
- MySQL installed and configured
- Pipenv installed

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/gct00/littlelemon-booking-api-django.git
   cd littlelemon-booking-api-django
   ```

2. **Activate the virtual environment**
   ```bash
   pipenv shell
   ```

3. **Install dependencies**
   ```bash
   pipenv install django
   pipenv install mysqlclient
   ```

4. **Configure MySQL database**
   - Create a MySQL database
   - Configure credentials in `littlelemon/settings.py`

5. **Run migrations**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

6. **Start the server**
   ```bash
   python manage.py runserver
   ```

7. **Access the project**
   - Open your browser and go to: `http://127.0.0.1:8000/`

## 🎯 Features

- **Home page** - Restaurant presentation
- **About** - Information about Little Lemon
- **Menu** - Restaurant menu
- **Bookings** - Table reservation system
- **Reservations view** - Lists all bookings in JSON format

## 📁 Project Structure

```
littlelemon-booking-api-django/
├── littlelemon/           # Django project settings
│   ├── settings.py       # Project settings
│   ├── urls.py          # Main URLs
│   └── wsgi.py          # WSGI configuration
├── restaurant/           # Main application
│   ├── models.py        # Data models
│   ├── views.py         # Django views
│   ├── forms.py         # Forms
│   ├── urls.py          # Application URLs
│   ├── templates/       # HTML templates
│   └── static/          # Static files (CSS, JS, images)
├── manage.py            # Django management script
├── Pipfile              # Pipenv dependencies
└── README.md           # This file
```

## 🔧 Database Configuration

In the `littlelemon/settings.py` file, configure the MySQL database:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'littlelemon',
        'USER': 'root',
        'PASSWORD': '',  # Your MySQL password
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

## 📝 Usage

1. **Make a reservation:**
   - Go to the "Book" page in the menu
   - Fill out the form with your details
   - Click "Submit"

2. **View reservations:**
   - Go to the "Reservations" page in the menu
   - Reservations will be displayed in JSON format in the browser console

## 🤝 Contributing

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## 👨‍💻 Author

**Guilherme Campion** - [GitHub](https://github.com/gct00)

---

**Developed as part of the Coursera Full Stack Development course** 