# Bookstore E-Commerce Website

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <h3 align="center">Bookstore</h3>

  <p align="center">
    An awesome e-commerce website for books.
    <br />
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#running-this-project">Running this project</a>
    </li>
  </ol>
</details>


## About The Project
<br>

This is a fully functional e-commerce website for books designed and developed as a full-stack web development project. This project is developed using Python Django framework as backend language, SQLite/PostgreSQL as database and other tools like HTML, CSS, Bootstrap and JavaScript.

- Modern and minimalistic design that appeals to the user.
- Guest user functionality for improved user experience.
- Custom Admin panel for advanced application management.
- Used Twilio API for OTP authentications and Razorpay for payment.

<br>

### Built With

![Python](https://img.shields.io/badge/Python%20-%2314354C.svg?style=for-the-badge&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5%20-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS%20-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)

<br>

## Running this project

To get this project up and running you should start by having Python installed on your computer. It's advised you create a virtual environment to store your projects dependencies separately. You can install virtualenv with

```
pip install virtualenv
```

Clone or download this repository and open it in your editor of choice. In a terminal (mac/linux) or windows terminal, run the following command in the base directory of this project

```
virtualenv venv
```

That will create a new folder `venv` in your project directory. Next activate it with this command on mac/linux:

```
source venv/bin/activate
```

On Windows:
```
venv\Scripts\activate
```

Then install the project dependencies with

```
pip install -r requirements.txt
```

Set up a `.env` file in the below format (optional for basic setup):
```
SECRET_KEY= <your_django_secret_key>
DEBUG= <True or False>

DATABASES_NAME= <your_database_name>
DATABASES_PASSWORD= <your_database_password>

EMAIL_HOST_USER= <email_from_which_all_mail_to_be_sent>
EMAIL_HOST_PASSWORD= <app_password_for_your_mail>

RAZORPAY_SECRET_KEY= <your_razorpay_secret_key>
RAZORPAY_KEY_ID= <your_razorpay_key_id>

TWILIO_ACCOUNT_SID= <your_twilio_account_sid>
TWILIO_AUTH_TOKEN= <your_twilio_auth_token>
```

Apply migrations and create your database
```
python manage.py migrate
```

Create a superuser with manage.py
```
python manage.py createsuperuser
```

Now you can run the project with this command

```
python manage.py runserver
```

The project will be available at `http://localhost:8000/`

<br>

## Features

- User authentication (Email verification, OTP login)
- Product browsing and search
- Shopping cart functionality
- Order management
- Admin dashboard
- Payment integration (Razorpay)
- Email notifications
