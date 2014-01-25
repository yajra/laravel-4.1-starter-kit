## Laravel 4.1 - Starter Kit with Oracle DB Support
This is a Laravel 4.1 Starter Kit and it will help you getting started with Laravel 4.1.

Tottaly based on [laravel4-starter-kit](https://github.com/brunogaspar/laravel4-starter-kit)


It includes examples on how to use the framework itself and how to use some
packages, like the awesome [Sentry 2](https://github.com/cartalyst/sentry) package.

-----

## Included goodies

* Twitter Bootstrap 2.3.2
* jQuery 1.10.2
* Custom CLI Installer
* Custom Error Pages:
	* 403 for forbidden page access
	* 404 for not found pages
	* 500 for internal server errors
	* 503 for the maintenance page
* Back-end
	* User and Group management
	* Manage blog posts and comments
* Front-end
	* User login, registration, activation and forgot password
	* User account area
	* Blog functionality with commentaries
	* Contact us page
* Packages included:
	* [Cartalyst Sentry 2 - Authentication and Authorization package](https://github.com/cartalyst/sentry)

-----

## Requirements

- PHP 5.3.7 or later
- MCrypt PHP Extension
- OCI8 PHP Extension (if you will user Oracle DB)

-----

## How to Install

### 1) Downloading
#### 1.1) Clone the Repository

	git clone https://github.com/yajra/laravel-4.1-starter-kit.git

#### 1.2) Download the Repository

	https://github.com/yajra/laravel-4.1-starter-kit-/archive/master.zip
-----

### 2) Install the Dependencies via Composer
##### 2.1) If you don't have composer installed globally

	cd your-folder
	curl -s http://getcomposer.org/installer | php
	php composer.phar install

##### 2.2) For globally composer installations

	cd your-folder
	composer install

-----

### 3) Setup Database

Now that you have the Starter Kit cloned and all the dependencies installed, you need to create a database and update the file `app/config/database.php`.

-----

### 4) Setup Mail Settings

Now, you need to setup your mail settings by just opening and updating the following file `app/config/mail.php`.

This will be used to send emails to your users, when they register and they request a password reset.

-----

### 5) Make sure app/storage is writable by your web server.

If permissions are set correctly:

	chmod -R 775 app/storage

Should work, if not try

	chmod -R 777 app/storage
-----


### 6) Use custom CLI Installer Command

Now, you need to create yourself a user and finish the installation.

Use the following command to create your default user, user groups and run all the necessary migrations automatically.

	php artisan app:install

-----

### 7) Accessing the Administration

To access the administration page, you just need to access `http://your-host/public/admin` on your browser and it will automatically redirect you to the login page, in the login page, just fill in and submit the form.

After you being authenticated, you will be redirected back to the administration page.

-----

### 8) LICENSE

This is free software distributed under the terms of the MIT license

### 9) Additional information

Inspired by and based on laravel4-starter-kit (https://github.com/brunogaspar/laravel4-starter-kit)
