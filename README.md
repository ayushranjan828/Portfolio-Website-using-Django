# Portfolio Website

A modern, responsive portfolio website built with Django. Showcase your skills, projects, and experience with a clean, professional design.

## 🚀 Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI**: Clean, professional design with smooth animations
- **Contact Form**: Built-in contact functionality
- **SEO Friendly**: Optimized for search engines
- **Fast Loading**: Optimized static files and efficient code structure

## 🛠️ Technologies Used

- **Backend**: Django 6.0.4
- **Frontend**: HTML5, CSS3, JavaScript
- **Database**: SQLite3 (development) / PostgreSQL (production)
- **Styling**: Custom CSS with responsive design
- **Deployment**: Ready for Heroku, DigitalOcean, or any Django-compatible hosting

## 📋 Prerequisites

Before running this project, make sure you have the following installed:

- Python 3.8 or higher
- pip (Python package installer)
- Git

## 🔧 Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/portfolio-website.git
   cd portfolio-website
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   # On Windows
   venv\Scripts\activate
   # On macOS/Linux
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply database migrations**
   ```bash
   python manage.py migrate
   ```

5. **Collect static files**
   ```bash
   python manage.py collectstatic --noinput
   ```

6. **Create a superuser (optional)**
   ```bash
   python manage.py createsuperuser
   ```

7. **Run the development server**
   ```bash
   python manage.py runserver
   ```

8. **Open your browser and visit** `http://127.0.0.1:8000/`

## 📁 Project Structure

```
portfolio-website/
├── myproject/                 # Main Django project directory
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py           # Django settings
│   ├── urls.py               # Main URL configuration
│   └── wsgi.py
├── portfolio/                 # Portfolio app
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py             # Database models
│   ├── tests.py
│   ├── urls.py               # App URL patterns
│   ├── views.py              # View functions
│   └── migrations/           # Database migrations
├── static/                   # Static files (CSS, JS, Images)
│   └── css/
│       └── style.css
├── templates/                # HTML templates
│   ├── base.html            # Base template
│   ├── home.html            # Home page
│   ├── about.html           # About page
│   ├── contact.html         # Contact page
│   └── includes/            # Template includes
│       ├── navbar.html
│       └── footer.html
├── db.sqlite3               # SQLite database (development)
├── manage.py               # Django management script
├── requirements.txt         # Python dependencies
└── README.md               # Project documentation
```

## 🎨 Customization

### Changing Colors and Styling
Edit `static/css/style.css` to customize:
- Color scheme
- Typography
- Layout spacing
- Responsive breakpoints

### Adding New Pages
1. Create new HTML template in `templates/`
2. Add URL pattern in `portfolio/urls.py`
3. Create view function in `portfolio/views.py`
4. Update navigation in `templates/includes/navbar.html`

### Adding Projects
Edit the projects section in your templates to showcase your work:
- Project images in `static/images/`
- Project descriptions and links
- Technologies used

## 🚀 Deployment

### Heroku Deployment
1. Create a Heroku app
2. Set environment variables:
   - `DEBUG=False`
   - `SECRET_KEY=your-secret-key`
   - `ALLOWED_HOSTS=your-app-name.herokuapp.com`
3. Push to Heroku:
   ```bash
   git push heroku main
   ```

### Local Production Setup
1. Set `DEBUG=False` in settings.py
2. Configure `ALLOWED_HOSTS`
3. Use a production database (PostgreSQL recommended)
4. Set up a web server (Nginx + Gunicorn)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes and commit: `git commit -am 'Add feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📧 Contact

Feel free to reach out if you have any questions or suggestions!

- **Email**: your.email@example.com
- **LinkedIn**: [Your LinkedIn](https://linkedin.com/in/yourprofile)
- **GitHub**: [Your GitHub](https://github.com/yourusername)

---

⭐ **Star this repo** if you found it helpful!
