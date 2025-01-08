# Installation
* Delete any previously cloned repo. (If any)
	`crustdata`
* Clone the repository.
    `git clone https://github.com/snaazze/crustdata.git`
* Go to the repository.
	`cd crustdata`
* Create a virtual environment.
	`virtualenv -p "[path to python3.exe]" python3.13`
	See below for instructions.
* Activate virtual environment.
	`python3.13\Scripts\activate`
* Install packages.
	`pip install -r requirements.txt`
* Go to app directory.
    `cd app`
* For Password Reset Functionality, add environment variables:
	`EMAIL_USER: email_address`
	`EMAIL_PASS: email_password`
	Avoid if not using password reset!!
* Migrate DB.
	`python manage.py migrate`
* Run server.
	`python manage.py runserver`
* Visit site at:
	`127.0.0.1:8000`

# Install Python 3.13 and create virtual environment for the same.
* Download Python 3.13 
	`https://www.python.org/ftp/python/3.13.1/python-3.13.1-amd64.exe`
* Install using the installer.
* In the start menu search for Python 3.13. In the option `Python 3.13 (64-bit)` right-click and go to file location. There is a shortcut with the same name `Python 3.13 (64-bit)`. Right-click on it and go to properties. In the properties, copy the value in the `Target` field.
* In the boot-up folder, create virtual environment
	`virtualenv -p [the value copied above] python3.13`
* Activate the virtual environment.
	`python3.13\Scripts\activate`