# First-Django-Project

# First Django Project

A minimal Django web application that serves a basic "Hello, World!" homepage. This project demonstrates the core concepts of Django URL routing and views.

## Features
* **Custom View:** A simple `home_page_view` that returns a plain text HTTP response.
* **App-Level Routing:** Clean URL routing configured directly inside the application's own `urls.py`.

---

## How to Run the Project Locally

Follow these steps to get the development server up and running on your machine.

### 1. Clone the Repository
```bash
git clone [https://github.com/anujbashyal/First-Django-Project.git](https://github.com/anujbashyal/First-Django-Project.git)
cd First-Django-Project

# On macOS/Linux:
source venv/bin/bin/activate

# On Windows:
.\venv\Scripts\activate

# On macOS/Linux:
source venv/bin/bin/activate

# On Windows:
.\venv\Scripts\activate

python manage.py runserver

from django.shortcuts import render
from django.http import HttpResponse

def home_page_view(request):
    return HttpResponse("Hello,World!")

from django.urls import path
from .views import home_page_view

urlpatterns = [
    path("", home_page_view),
]

