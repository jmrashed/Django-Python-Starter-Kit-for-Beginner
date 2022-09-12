# Django-Python-Starter-Kit-for-Beginner

Django was invented by Lawrence Journal-World in 2003, Initial release to the public was in July 2005. Latest version of Django is 4.0.3 (March 2022).

## What is Django?

Django is a Python framework that makes it easier to create web sites using Python. Django takes care of the difficult stuff so that you can concentrate on building your web applications.

## How does Django Work?

Django follows the MVT design pattern (Model View Template).

- Model - The data you want to present, usually data from a database.
- View - A request handler that returns the relevant template and content - based on the request from the user.
- Template - A text file (like an HTML file) containing the layout of the web page, with logic on how to display the data.

### Model

In Django, the data is delivered as an Object Relational Mapping (ORM). The most common way to extract data from a database is SQL. Django, with ORM, makes it easier to communicate with the database, without having to write complex SQL statements.

The models are usually located in a file called `models.py`.

### View

A view is a function or method that takes http requests as arguments, imports the relevant model(s), and finds out what data to send to the template, and returns the final result.

The views are usually located in a file called `views.py`.

### Template

Templates are often .html files, with HTML code describing the layout of a web page, but it can also be in other file formats to present other results, but we will concentrate on .html files.
Django uses standard HTML to describe the layout, but uses Django tags to add logic:

```python
<p>My name is {{ firstname }}.</p>
```

The templates of an application is located in a folder named `templates`.

### URLs

Django also provides a way to navigate around the different pages in a website. When a user requests a URL, Django decides which view it will send it to.

This is done in a file called `urls.py`.

## Django Requires Python

To check if your system has Python installed, run this command in the command prompt:

```
PS C:\Users\Jmrashed> python --version
PS C:\Users\Jmrashed> Python 3.10.6
```

If you find that you do not have Python installed on your computer, then you can download it for free from the following website: https://www.python.org

## Django Requires PIP (package manager)

To install Django, you must use a package manager like PIP, which is included in Python from version 3.4.To check if your system has PIP installed, run this command in the command prompt:

```
PS C:\Users\Jmrashed> pip --version
pip 22.2.2 from C:\Users\Jmrashed\AppData\Local\Programs\Python\Python310\lib\site-packages\pip (python 3.10)
```

If you do not have PIP installed, you can download and install it from this page: https://pypi.org/project/pip

## Django Virtual Environment

It is suggested to have a dedicated virtual environment for each Django project, and one way to manage a virtual environment is venv, which is included in Python.

`py -m venv myproject`

This will set up a virtual environment, and create a folder named "myproject" with subfolders and files, like this:

```
myproject
  Include
  Lib
  Scripts
  pyvenv.cfg
```

Then you have to activate the environment, by typing this command:
`myproject\Scripts\activate.bat`

## Install Django

Finally, we can install Django. Django is installed using pip, with this command:

`(myproject) C:\Users\Jmrashed> py -m pip install Django`

## Check Django Version

You can check if Django is installed by asking for its version number like this:

`(myproject) C:\Users\Jmrashed>django-admin --version`
If Django is installed, you will get a result with the version number:
`4.0.3`
