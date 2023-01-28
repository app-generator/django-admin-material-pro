# **[Django Admin Material PRO](https://appseed.us/product/material-dashboard-pro/django/)**

**Django** starter styled with **[Django Admin Material PRO](https://appseed.us/product/material-dashboard-pro/django/)**, a premium `Bootstrap` design from [Creative-Tim](https://bit.ly/3fKQZaL).
The product is designed to deliver the best possible user experience with highly customizable feature-rich pages. 

> 👉 **NOTE**: This product `requires a License` in order to access the theme:

**Private REPO**: `git+https://github.com/app-generator/priv-django-admin-argon-pro`

<br />

## Features: 

- **UI Kit**: Material Dashboard PRO `v2.2.2` by Creative-Tim 
- [Django Material PRO](https://github.com/app-generator/django-material-dashboard-pro) - `sample project`
- **Sections Covered**: 
  - `Admin Section`, reserved for `superusers`
  - `All pages` managed by `Django.contrib.AUTH`
  - `Registration` page
  - `Misc pages`: colors, icons, typography, blank-page 

<br />

![Material Dashboard BS4 PRO](https://user-images.githubusercontent.com/51070104/214523237-e71b66e6-4db6-4467-a4c2-550c37de7553.png)

<br />

## Why `Django Admin Material PRO`

- Modern [Bootstrap](https://www.admin-dashboards.com/bootstrap-5-templates/) Design
- `Responsive Interface`
- `Minimal Template` overriding
- `Easy integration`

**Material Dashboard PRO** makes use of light, surface and movement. The general layout resembles sheets of paper following multiple layers, so that the depth and order is obvious. Inside the archive you will find multiple example pages on how to use all components.

<br />

## How to use it

<br />

> **Install the package** via `PIP` 

```bash
$ pip install git+https://github.com/app-generator/priv-django-admin-material-pro.git
```

<br />

> Add `admin_material_pro` application to the `INSTALLED_APPS` setting of your Django project `settings.py` file (note it should be before `django.contrib.admin`):

```python
    INSTALLED_APPS = (
        ...
        'admin_material_pro.apps.AdminMaterialProConfig',
        'django.contrib.admin',
    )
```

<br />

> Add `LOGIN_REDIRECT_URL` and `EMAIL_BACKEND` of your Django project `settings.py` file:

```python
    LOGIN_REDIRECT_URL = '/'
    # EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
    EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
```

<br />

> Add `admin_material_pro` urls in your Django Project `urls.py` file

```python
    from django.urls import path, include

    urlpatterns = [
        ...
        path('', include('admin_material_pro.urls')),
    ]
```

<br />

> **Collect static** if you are in `production environment`:

```bash
$ python manage.py collectstatic
```

<br />

> **Start the app**

```bash
$ # Set up the database
$ python manage.py makemigrations
$ python manage.py migrate
$
$ # Create the superuser
$ python manage.py createsuperuser
$
$ # Start the application (development mode)
$ python manage.py runserver # default port 8000
```

Access the `admin` section in the browser: `http://127.0.0.1:8000/`

<br />

---
**[Django Admin Material PRO](https://appseed.us/product/material-dashboard-pro/django/)** - Modern Admin Interface provided by **[AppSeed](https://appseed.us/)**
