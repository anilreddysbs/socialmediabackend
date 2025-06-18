# Social Media Backend

A backend API for a social media platform, built with Django and Django REST Framework. This project provides endpoints for user authentication, posting, commenting, and more.

## Features

- User registration and authentication
- Create, read, update, and delete posts
- Comment on posts
- Like and unlike posts
- User profiles
- RESTful API endpoints for integration with frontend apps

## Tech Stack

- Python
- Django
- Django REST Framework

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/anilreddysbs/socialmediabackend.git
   cd socialmediabackend
   ```

2. **Create and activate a virtual environment (recommended):**
   ```bash
   python -m venv venv
   # On Windows:
   venv\Scripts\activate
   # On macOS/Linux:
   source venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
   *(If `requirements.txt` is missing, install Django and Django REST Framework manually: `pip install django djangorestframework`)*

4. **Apply migrations:**
   ```bash
   python manage.py migrate
   ```

5. **Create a superuser (optional, for admin access):**
   ```bash
   python manage.py createsuperuser
   ```

6. **Run the development server:**
   ```bash
   python manage.py runserver
   ```

7. **API is available at:**  
   [http://127.0.0.1:8000/api/](http://127.0.0.1:8000/api/)  
   *(Adjust the URL based on your API routing.)*

## API Endpoints

- `POST /api/register/` — Register a new user
- `POST /api/login/` — User login
- `GET /api/posts/` — List all posts
- `POST /api/posts/` — Create a new post
- `GET /api/posts/<id>/` — Retrieve a specific post
- `PUT /api/posts/<id>/` — Update a post
- `DELETE /api/posts/<id>/` — Delete a post
- `POST /api/posts/<id>/comments/` — Add a comment to a post
- `POST /api/posts/<id>/like/` — Like a post
- `POST /api/posts/<id>/unlike/` — Unlike a post

*(Update these endpoints based on your actual API URLs.)*

## Usage

- Use tools like [Postman](https://www.postman.com/) or `curl` to interact with the API.
- Integrate with a frontend or mobile app for a complete social media experience.

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT](LICENSE)

---

*Build and extend your own social media backend with Django!*
