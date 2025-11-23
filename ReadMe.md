**Step 1**: Install Django

pip install django

**Step 2**: Create Django Project

django-admin startproject mysite

**Step 3**: Run Migrations

Create migration:

python manage.py makemigrations students

Apply to database:

python manage.py migrate

**Step 4**: Add Sample Data

Open Django shell:

python manage.py shell

Then insert data:

from students.models import Student
Student.objects.create(name="Niranjana", age=23, email="ni@example.com")
Student.objects.create(name="Arun", age=21, email="arun@example.com")
Student.objects.create(name="Priya", age=22, email="priya@example.com")

Exit shell:

exit()

**Step 5**: Run the Development Server
python manage.py runserver

**Step 6:** Server will start at:

👉 http://127.0.0.1:8000

👉 http://127.0.0.1:8000/students

To exit terminal: **Ctrl + C**