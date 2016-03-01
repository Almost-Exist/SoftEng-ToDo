<<<<<<< HEAD
# Python Starter Overview

The Python Starter demonstrates a simple, reusable Python web application.

## Run the app locally

1. [Install Python][]
2. Download and extract the starter code from the Bluemix UI
3. cd into the app directory
4. Run `python server.py`
5. Access the running app in a browser at http://localhost:8000

## About
A backend for the ToDo app written in Python.  ToDos is stored in 
Mongo DB.

## Prerequisites
Before running this app or deploying it to BlueMix you need to have 
[Python](https://www.python.org/), 
[PIP](http://www.pip-installer.org/), 
[Paver](http://paver.github.io/paver/), and the 
[CloudFoundry Command Line](https://github.com/cloudfoundry/cli) 
installed.

## Deploying To BlueMix

The Paver file takes care of everything you need to do to deploy to IBM BlueMix server, including 
creating and binding to the services.  Before you deploy the app please make sure you 
have all the prerequisites from the section above installed and working, they are used by 
the Paver tasks.

### Login To BlueMix From The Command Line

The Paver file contains a task that will do this for you, just run

    $ paver cf_login

You will be prompted to enter your BlueMix user name and password.



============ OR ===============



You can also do this by using the Cloud Foundry command line tool directly.

    $ cf login -a https://api.ng.bluemix.net

### Deploying To BlueMix


To deploy the app so it uses Mongo DB run

    $ paver deploy_mongo_todo

This tasks will prompt you for a name to use for your application.  The name must be unique, if it is
not unique the deploy will fail.  If it does fail run the task again and enter a different name.
=======
# SoftEng-ToDo
>>>>>>> 57a4600f178541b84b050900f38a66a3d55bb354
