# Django Concepts

## 1. Django Setup & Project Structure
   - **Django Project Setup**: Commands to create and start a new Django project and app, and how to run the server.
   - **Project Structure**: Understanding how Django organizes files and directories, such as `urls.py`, `views.py`, `models.py`, etc.

## 2. Django Models
   - **Model Creation**: Creating models in Django using the `models.Model` class (e.g., `CustomUser`, `Course`).
   - **ORM (Object-Relational Mapping)**: Using Django’s ORM to interact with the database (e.g., `CustomUser.objects.create()`).
   - **Field Types**: Understanding field types such as `CharField`, `TextField`, `URLField`, etc.
   - **Model Relationships**: Defining relationships between models using `ForeignKey` (e.g., in the `Progress` model).
   - **Migrations**: Applying migrations to create or update database tables (`python manage.py makemigrations` and `python manage.py migrate`).

## 3. User Authentication & JWT
   - **Custom User Model**: Creating a custom user model by extending `AbstractUser` for user management.
   - **Authentication**: Using Django's built-in authentication system for user management.
   - **JWT (JSON Web Tokens)**: Integrating JWT-based authentication with `djangorestframework-simplejwt` to manage user login and token-based authentication.
   - **DRF (Django Rest Framework)**: Using Django Rest Framework for API development, including `TokenObtainPairView` for JWT token generation.

## 4. Django Views & REST APIs
   - **Views**: Creating views to handle requests and return responses, including custom views for login (`TokenObtainPairView`) and displaying data.
   - **API Views**: Creating API views for the frontend to interact with the backend (e.g., Course API, Quiz Generation API).
   - **Django Rest Framework (DRF)**: Using serializers, viewsets, and the DRF to create APIs efficiently.

## 5. Django Middleware
   - **Middleware**: Custom middleware for logging activities (`ActivityLogMiddleware`) and processing requests before passing them to views.
   - **Request/Response Cycle**: Understanding how middleware interacts with the request/response cycle and modifying request/response behavior.

## 6. Django REST Framework (DRF)
   - **ViewSets & Serializers**: Using viewsets (`ModelViewSet`) and serializers (`CourseSerializer`) for managing data in API endpoints.
   - **Authentication Classes**: Configuring JWT authentication with DRF’s settings (`DEFAULT_AUTHENTICATION_CLASSES`).

## 7. Database Integration
   - **SQLite/MongoDB**: Working with different databases (SQLite for initial development and MongoDB for activity logging).
   - **pymongo**: Integrating MongoDB using `pymongo` for logging and tracking user activity.

## 8. Backend Logic
   - **Business Logic**: Implementing business logic for course recommendations based on user activities or other criteria.
   - **Database Queries**: Writing queries to retrieve data based on certain conditions (e.g., fetching recommended courses based on user activity).

## 9. Celery for Asynchronous Tasks
   - **Celery**: Using Celery for background tasks such as sending notifications for progress tracking.

## 10. Deployment
   - **Deployment with Gunicorn**: Deploying the Django application using Gunicorn as the WSGI server.
   - **Heroku Deployment**: Deploying the Django application to Heroku for production.
   - **Static & Media Files**: Handling static files and media during deployment.

## 11. Testing & Debugging
   - **Django Shell**: Using `python manage.py shell` to interact with the Django ORM and test code snippets.
   - **Unit Testing**: Writing tests for views, models, and other Django components to ensure the application behaves as expected.

## 12. Frontend-Backend Communication
   - **Cross-Origin Resource Sharing (CORS)**: Although not explicitly mentioned, CORS may need to be handled for communication between the Django backend and React frontend.
   - **API Integration**: Connecting the React frontend with Django's backend using Axios to fetch and send data (e.g., logging in, fetching course data).
