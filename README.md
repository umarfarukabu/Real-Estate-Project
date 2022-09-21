# Real-Estate-Project

A real estate listings website built with `python` `django` `bootstrap`.

A simple, reponsive  website. Built with:

- Python 🐍
- Django 🎸
- Bootstrap 4 🌈
- Vanilla JS - ES6
- JQuery

## How to run this project (Ubuntu 18.04)

1. **Clone the project**

```sh
git clone https://github.com/umarfarukabu/Real-Estate-Project.git
```

2.  **Make sure you are in *Real-Estate-Django-Web-App* folder**

   1. Install all dependencies

      ```sh
      pip install -r requirements.txt
      ```

3. **Install PostgreSQL in your Ubuntu 18.04**

   1. Enable PostgreSQL Apt Repository

      ```sh
      sudo apt-get install wget ca-certificates
      
      wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
      
      # Now add the repository to your system.
      
      sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" >> /etc/apt/sources.list.d/pgdg.list'
      ```

   2. Install PostgreSQL on Ubuntu

      ```sh
      sudo apt-get update
      sudo apt-get install postgresql postgresql-contrib
      ```

   3. Connect to PostgreSQL

      ```sh
      sudo su - postgres
      psql
      ```

      Now you are logged in to PostgreSQL database server. To check login info use following command from the database command prompt.

      ```sh
      postgres-# \conninfo
      ```

   4. Create a database

      ```sh
      CREATE DATABASE real_estate;
      ```

   5. Create user 

      ```sh
      CREATE USER pks WITH PASSWORD 'abc123!';
      ```
   
4. **Run Migrations**

```sh
python manage.py makemigrations
python manage.py migrate
```

5. **Run Server**
```sh
python manage.py runserver 
```

And you are good to go. 



**Backend**

For Database I have used Postgres Database Name: real_estate

Note: Please change those gmail credentials from real_estate folder you will get settings.py inside that file you will see username and password mentioned as place your Username and Password. Also do that same thing from Contacts folder views.py you will see YourEmail mentioned on line number 33.

### Screenshots

- **HOME**

![Home](https://github.com/TheCaffeineDev/Real-Estate-Django-Web-App/blob/master/screenshots/s1.JPG)

- **Listings** 


![Listings](https://github.com/TheCaffeineDev/Real-Estate-Django-Web-App/blob/master/screenshots/s3list.JPG)

- **Registration** 

![Registration](https://github.com/TheCaffeineDev/Real-Estate-Django-Web-App/blob/master/screenshots/s4reg.JPG)

- **Admin Panel - 1**

![Admin](https://github.com/TheCaffeineDev/Real-Estate-Django-Web-App/blob/master/screenshots/s5adm.JPG)

- **Admin Panel - 2**

![Admin](https://github.com/TheCaffeineDev/Real-Estate-Django-Web-App/blob/master/screenshots/s6r.JPG)

- **About**

![About ](https://github.com/TheCaffeineDev/Real-Estate-Django-Web-App/blob/master/screenshots/s2about.JPG)
