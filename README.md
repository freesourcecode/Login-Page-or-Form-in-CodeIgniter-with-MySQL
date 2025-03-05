# Login Page or Form in CodeIgniter With MySQL with Source Code

A user can access an application through the Login Page or Form in CodeIgniter by entering their username and password or by logging in with a social media account.

## About the Project

The **Login Page (Form) in CodeIgniter** with Database was developed using CodeIgniter and MySQL Database as Back-End.

In this article, we’ll learn how to use CodeIgniter to create a Session in CodeIgniter for Login.

We created a login module in the login form.

A **Login Form in CodeIgniter** with Session, By providing a valid username and password, you can log in. If an invalid login or password is entered, an error message will appear.

## What is CodeIgniter?
**CodeIgniter** is an Application Development Framework – a toolset – for PHP website developers.

Its purpose is to let you construct projects much faster than if you were programming code from the start by providing a rich set of libraries for common activities, as well as a simple interface and logical structure to access these libraries.

By reducing the amount of code required for a given operation, CodeIgniter allows you to focus more creatively on your project.

In this Login Query In CodeIgniter also includes a downloadable Login In CodeIgniter With Session free source code, just find the downloadable source code below and click to start downloading.

To start executing this **Login Page in CodeIgniter With Database**, make sure that you have sublime or any platform of PHP and MySQL installed on your computer.

## How to run the CodeIgniter Login Page or Form? A Step-by-step Tutorial with Source Code

These are the steps on how to run the **Login Page in CodeIgniter with Database Source Code**.

1. **Download Source Code**

2. **Extract File**

Next, after finishing downloading the file, go to the file location and right click the file and click extract.
login page extract file

![image](https://github.com/user-attachments/assets/91c84a6d-6c7d-414e-ba72-0987b7501fa3)

3. **Copy Project Folder**

Copy the project folder and paste it to C:\xampp\htdocs.

4. **Open Xampp**
Next, open xampp and start the apache and mysql.

5. **Create Database**

Click any browser type the URL localhost/phpmyadmin, and create a database.

![image](https://github.com/user-attachments/assets/708d87fa-a504-4847-a87d-50132aa29842)

6. **Import Database**

Click the created database, click import to the right tab, click choose file, and import the sql file inside the download folder.

![image](https://github.com/user-attachments/assets/a7a713b0-07db-4f45-9028-97b0b086d489)

7. **Execute Project**
Lastly, type to the URL localhost/codeigniter_login.

## How to Create a Login Page or Form in CodeIgniter With MySQL?

The code given below is for the login page module

### views: login_page.php

``` <!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<title>CodeIgniter Login (IT SOURCECODE)</title>
	<link rel="stylesheet" type="text/css" href="<?php echo base_url(); ?>bootstrap/css/bootstrap.min.css">
</head>
<body class="bg-info">
<div class="container">
	<h1 class="page-header text-center">CodeIgniter Login (IT SOURCECODE)</h1>
	<div class="row">
		<div class="col-sm-4 col-sm-offset-4">
			<div class="login-panel panel panel-success">
		        <div class="panel-heading">
		            <h3 class="panel-title"><span class="glyphicon glyphicon-lock"></span> Login
		            </h3>
		        </div>
		    	<div class="panel-body">
		        	<form method="POST" action="<?php echo base_url(); ?>index.php/user/login">
		            	<fieldset>
		                	<div class="form-group">
		                    	<input class="form-control" placeholder="Email" type="email" name="email" required>
		                	</div>
		                	<div class="form-group">
		                    	<input class="form-control" placeholder="Password" type="password" name="password" required>
		                	</div>
		                	<button type="submit" class="btn btn-lg btn-success btn-block"><span class="glyphicon glyphicon-log-in"></span> Login</button>
		            	</fieldset>
		        	</form>
		    	</div>
		    </div>
			<?php
				if($this->session->flashdata('error')){
					?>
					<div class="alert alert-danger text-center" style="margin-top:20px;">
						<?php echo $this->session->flashdata('error'); ?>
					</div>
					<?php
				}
			?>
		</div>
	</div>
</div>
</body>
</html>
```

### Login Page Output:

![image](https://github.com/user-attachments/assets/d722f3a2-f9e7-4162-b670-646de67fe410)

The code given below is for the home module

### views: home.php

```<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<title>CodeIgniter Login</title>
	<link rel="stylesheet" type="text/css" href="<?php echo base_url(); ?>bootstrap/css/bootstrap.min.css">
</head>
<body>
<div class="container">
	<h1 class="page-header text-center">CodeIgniter Login with Flashdata</h1>
	<div class="row">
		<div class="col-md-4 col-md-offset-4">
			<?php
				$user = $this->session->userdata('user');
				extract($user);
			?>
			<h2>Welcome to Homepage </h2>
			<h4>User Info:</h4>
			<p>Fullname: <?php echo $fname; ?></p>
			<p>Email: <?php echo $email; ?></p>
			<p>Password: <?php echo $password; ?></p>
			<a href="<?php echo base_url(); ?>index.php/user/logout" class="btn btn-danger">Logout</a>
		</div>
	</div>
</div>
</body>
</html>
```

### Homepage Output:

![image](https://github.com/user-attachments/assets/2dd88008-7b78-4ab5-97fa-78420510287d)

### 📌 Here's the full documentation for the [Login Page or Form in CodeIgniter With MySQL](https://itsourcecode.com/free-projects/php-project/login-page-in-codeigniter-with-database/)
