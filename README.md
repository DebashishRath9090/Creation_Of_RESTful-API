# Creation_Of_RESTful-API
                   -------------------------Documentation for Running and Testing this project-----------------------------

--> Hi !! My name is Debashish Rath.
--> In this document I'll brief about this project and state the important instructions for proper running and testing this Project.

Briefing about the Project:

* This project is all about creating a RESTful API by using Python Programming Language along with MySQL Database for storing data.

* Version of Python used: Python 3.9

* Here, "flask" microframework of Python has been used.



Project requirement:

* Latest version of Python should be installed in the system and environment variable path should be   specified properly.

* Few modules are required to be installed, which are listed below:
	. flask
	. flask-restful
	. pymysql
	. flaskext
	. Flask-MySQL

	Steps to install these:
	. Go to Command Prompt (for Windows users)
	. type this command there: pip install module_name_from_above_list_which_you_wanna_install
	. If you have these modules installed previously, then it will give you message as "Requirement already satisfied."
	. Else, you will get message as "Successfully installed."




Steps to follow for optimal running and testing this project:

--> In this project, along with this documentation you will get three Python files (files having .py extension) and one MySQL_database_Schema folder, from where you will get two .sql files.



--> Three Python files are:
	. Coditation Project.py
	. app.py
	. sys_config.py


--> Ensure that you have the database_schema which has been provided, before starting the further process.


--> In sys_config.py file, you need to configure the database by giving required inputs.
    
--> You will get following fields in this Python file:
	. MySQL configurations
	--> app.config['MYSQL_DATABASE_USER'] = ""
	--> app.config["MYSQL_DATABASE_PASSWORD"] = ""
	--> app.config["MYSQL_DATABASE_DB"] = "the_tech_world_store"
	--> app.config["MYSQL_DATABASE_HOST"] = "" 

	# Here, you need to enter your database username, password and host.
	# The name of my database_schema here is "the_tech_world_store", so I have written above as it is.
	# Remaining fields are to be filled by you.
	

--> In order to start the flask server, please run the command "python Coditation Project.py".

--> For API testing you can use Postman, Talend API Tester (It has chrome extension)

--> The endpoints for testing various HTTP methods:

	. GET	  -->	"/my_tech_store" 
			"/my_tech_store/product"                        						
			"/my_tech_store/category"
			"/my_tech_store/category/Category_ID"                         						
			"/my_tech_store/product/Product_ID"

	. POST	  -->	"/add/category"
			"/add/product"

	. PUT	  -->	"/update/category"
			"/update/product"

	. DELETE  -->	"/delete/category/Category_ID"
			"/delete/product/Product_ID"


--> For adding and updating "Product" data and "Category" data, you can refer to the format provided inside two text files which are "Product_file.txt" and "Category_file.txt".

--> You can test these operations by using above formats.


----------------------------------------------Thank You-------------------------------------------------
