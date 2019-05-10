# Setting Up Laravel

Simple steps to use when setting up Laravel environment for PHP


## Installing Server Requirements:

#### Ensure you have PHP7.0+ installed in your computer. install by running this command

`$ sudo apt install php7.2-cli`

#### Ensure you have the following server Requirements that don't come when installing php7.2:

###### Mbstring PHP Extension

`$ sudo apt-get install php-mbstring`

###### XML PHP Extension

`$ sudo apt-get install php-xml`

###### BCMath PHP Extension

`$ sudo apt install php7.2-bcmath`

## Download Composer:

This is what will be managing your php dependencies for your application, run the 4 commands in the link respectively for this purpose.

 (<https://getcomposer.org/download/>)

To confirm if composer has been installed run the following to check composer version

`$ composer`

If you get an error stating that 'composer command not found', run the following command:

`$ chmod +x composer.phar`

## Set PATH variable:

#### Run this command be able to export the PATH

`$ nano ~/.bashrc`

#### Then add the following line of code at the bottom of the files and save it

`$HOME/.config/composer/vendor/bin`

#### Then run the following

  `$ source ~/.bashrc`  

## Setting Up Apache server:

`$ sudo apt-get update`

`$ sudo apt-get install apache2`

#### To check if the server is set up, cd into

`$ cd /var/www/html`

## download the Laravel installer using Composer:

`$ sudo apt-get install php7.2-zip`

`$ composer global require laravel/installer`  

## Create a Laravel project:

`$ laravel new blog`

or

`$ composer create-project --prefer-dist laravel/laravel blog`

then finally

`$ cd blog`

#### To run the server, run this commands

`$ php artisan serve`
