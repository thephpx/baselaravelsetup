# Development Manual
This file will outline the possible configuration of this base laravel setup.

## Initialization
At first create the `dist` directory by creating laravel application via composer. 
> composer create-project --prefer-dist laravel/laravel dist

Next setup the database by giving `root` as user and `<blank>` password in `.env` file. 

Login using the remote mysql admin user to create the database. You can find the admin user's random password by running docker without deamon mode using `docker-compose up`. This will show the random password generated in terminal when running for first time. Save the password in a local file for future local development.

Now you got a fresh laravel setup running.

## Setting up voyager admin panel

This setup expects to use voyager as laravel admin panel. 
* > composer require tcg/voyager
* > php artisan voyager:install
* > php artisan voyager:admin admin@example.com --create 
* > The default url for admin is `localhost/admin`


## Config
* Database username is `root` & password is `<blank>`. By default the root user only accessible from within the system. 
