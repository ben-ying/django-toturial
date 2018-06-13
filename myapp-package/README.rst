=====
myapp-package
=====

myapp-package is a simple Django app package. For each question, visitors can choose between a fixed number of answers.

Detailed documentation is in the "docs" directory.

Quick start
-----------

1. Add "myapp-package" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'myapp-package',
    ]

2. Include the URLconf in your project urls.py like this::
    path('myapp/', include('myapp.urls')),

3. Run `python manage.py migrate` to create the models.

4. Start the development server and visit http://127.0.0.1:8000/admin/              to create a model (you'll need the Admin app enabled).

5. Visit http://127.0.0.1:8000/myapp/ to participate in the model.
