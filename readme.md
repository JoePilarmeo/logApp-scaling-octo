# **Log App Tracking System**

LogApp is a user-friendly web application that helps users manage their logs easily. It has four PHP files: an index, login, logout, and a list file. Users can add new logs by registering on the index page, admin can login in the login page and see the list page that organize logs by date together with logout button. To use the app, users need to set up a MySQL database using remote tools such as Workbench or phpMyAdmin. This repository will provide clear instructions to guide users through the database setup process.

## Visuals

![Index Page](https://i.pinimg.com/originals/79/1d/59/791d59dd97d1493054dc24e8be013eaa.jpg)

![Login Page](https://i.pinimg.com/originals/35/1a/a4/351aa44471511dfceb79ad98884b0ed9.jpg)

![List Page](https://i.pinimg.com/originals/89/66/cb/8966cb580143cb8211b8ecbde0edb1c3.jpg)

___

### Requirements

- [Xampp](https://www.apachefriends.org/download.html)
- [Gitbash](https://git-scm.com/downloads) (*Optional: if you want to clone this project or [Download ZIP](https://github.com/JoePilarmeo/logApp-scaling-octo/archive/refs/heads/main.zip)*)
- [Workbench](https://dev.mysql.com/downloads/workbench/) (*Optional: if you don't want to use phpmyadmin*)

> You can clone or [Download ZIP](https://github.com/JoePilarmeo/logApp-scaling-octo/archive/refs/heads/main.zip) to make the local copy of this project

## Installation

**Cloning a repository**
1. Open gitbash and navigate htdocs by typing this code `cd C:/xampp/htdocs`
2. Now make a copy of it by typing this code `git clone (repository_link)`

**ZIP Download**
Extract this ZIP file in `cd C:/xampp/htdocs` directory  


 Now you have a local copy of this project! We are now going to prepare the database remotely, follow these steps:


1. First, open xampp and click "Start" under the "Apache" and "MySQL".

2. Create empty database and import the `log-app-scaling-octo.sql`

***Using phpmyadmin***

- Go to your browser and copy paste this url `http://localhost/phpmyadmin`.
- After that create a new database at the right navigation panel click "New", input the database name `log-app-scaling-octo` and click "Create".
- Click the "Import" window at the top, click the "Choose file", navigate the backup file in the local project that has this name `log-app-scaling-octo.sql` in folder of database and click "Import".

***Using workbench***
- Open the Mysql Workbench connect to your MySQL server.
- In the Navigator panel, right-click on the MySQL server instance and select "Create Schema..." from the context menu.	
- Enter the name of your schema then click the apply button
- Click on "Server" in the top menu and select "Data Import".
- In the "Data Import" window, select "Import from Self-Contained File" and select the backup file that has `log-app-scaling-octo.sql` in the database folder at the root directory of the project.
-Now click the "Start Import".

3. After importing the `log-app-scaling-octo.sql` file, you need to update the database credentials in the config.php file to match your own database setup. The config.php file is located in the config folder of this repository.
4. Open the config.php file and locate the following lines of code:

        define('ROOT_URL', '');
	    define('DB_HOST', '');
	    define('DB_USER', '');
	    define('DB_PASS', '');
	    define('DB_NAME', '');
        
5. Replace the values for DB_HOST, DB_NAME, DB_USER, and DB_PASSWORD with the credentials for your own database setup and save the config.php. 

6. Now all needed are set, check the website now if it is running sucessfully copy paste this url to your web browser `http://localhost/log-App-scaling-octo/`

## Authors
+ The author of this project are  
[JoePilarmeo](https://github.com/JoePilarmeo) :wink:

![Author 1](https://i.pinimg.com/originals/2a/ca/90/2aca9092e92d0216a813aa1aa8a980a5.jpg)

[MJRiego](https://github.com/MJRiego) :blush:

![Author 2](https://i.pinimg.com/originals/95/f3/10/95f310f128f57ff89f4a8ccaa117414e.jpg)

[MarkCreador](https://github.com/MarkCreador) :neutral_face:

![Author 3](https://i.pinimg.com/originals/e4/d5/33/e4d533dab632a47f70937f7a5a51921f.jpg)