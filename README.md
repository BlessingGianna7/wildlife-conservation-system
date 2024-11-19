# Wildlife Conservation System

This repository contains two independent backend implementations of a Wildlife Conservation System:
1. FastAPI Backend
2. Django Backend & Frontend

## Project Structure
wildlife-conservation-system/
├──wildlife-conservation-fastapi-backend/
│ └── app/
└──wildlife-conservation-django-backend/
└── project/

## Technologies Used
Django
FAST API
HTML
CSS

### FastAPI Backend
- Python 3.8+
- FastAPI
- SQLAlchemy
- Pydantic
- Uvicorn
- PostgreSQL/SQLite

### Django Backend
- Python 3.8+
- Django 5.1
- Django REST Framework
- SQLite/PostgreSQL

## Setup Instructions

### 1. Clone the Repository

https://github.com/BlessingGianna7/wildlife-conservation-system.git

cd wildlife-conservation-system


### 2. FastAPI Backend Setup

1. Create and activate a virtual environment:

python -m venv fastapi-env

# On Windows

fastapi-env\Scripts\activate

# On Unix or MacOS

source fastapi-env/bin/activate


2. Install dependencies:

cd fastapi-backend
pip install fastapi sqlalchemy pydantic uvicorn


3. Run the application:

uvicorn app.main:app --reload


4. Access the API:
- API endpoints: `http://127.0.0.1:8000`
- Interactive API documentation: `http://127.0.0.1:8000/docs`
- Alternative API documentation: `http://127.0.0.1:8000/redoc`

### 3. Django Backend Setup

1. Create and activate a virtual environment:

bash

python -m venv django-env

# On Windows

django-env\Scripts\activate

# On Unix or MacOS

source django-env/bin/activate


2. Install dependencies:

cd django-backend
pip install django djangorestframework

3. Apply migrations:

python manage.py migrate

4. Run the development server:

python manage.py runserver




5. Access the application at `http://127.0.0.1:8000`

## Features

### FastAPI Backend
- RESTful API endpoints for animals, guiders, and guests
- Many-to-many relationships between entities
- CRUD operations for all models
- Efficient database queries using SQLAlchemy

### Django Backend
- Full-featured web interface
- Authentication and authorization
- Statistics dashboard
- CRUD operations for animals, guests, and guides
- Form handling and validation

## API Documentation

### FastAPI Backend
Detailed API documentation is automatically generated and available at:
- Swagger UI: `http://127.0.0.1:8000/docs`
- ReDoc: `http://127.0.0.1:8000/redoc`

### Django Backend
Main URLs:
- Home: `/`
- Animals: `/animals/`
- Guests: `/guests/`
- Statistics: `/statistics/`

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the LICENSE file for details