# Class27 Reading Notes

## Readings: Django Models
Below you will find some reading material, code samples, and some additional resources that support today’s topic and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

## Reading
[Using Models](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models)

When designing your models it makes sense to have separate models for every "object" (a group of related information).

you might also want to use models to represent selection-list options (e.g. like a drop down list of choices), rather than hard coding the choices into the website itself — this is recommended when all the options aren't known up front or may change. 

Once we've decided on our models and field, we need to think about the relationships. Django allows you to define relationships that are one to one (OneToOneField), one to many (ForeignKey) and many to many (ManyToManyField).

## Models 
**Fields -** A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables.

**Metadata -** You can declare model-level metadata for your Model by declaring class Meta

**Methods -** A model can also have methods.

Minimally, in every model you should define the standard Python class method \__str__() to return a human-readable string for each object. 

**Model management -** Once you've defined your model classes you can use them to create, update, or delete records, and to run queries to get all records or particular subsets of records.

[Django Admin](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site)

Advanced configuration section is optional

The tutorial is really good but some of the tools are dated so when reading try to understand the concepts more than the code.

The Django admin application can use your models to automatically build a site area that you can use to create, view, update, and delete records.
All the configuration required to include the admin application in your website was done automatically when you created the skeleton project (for information about actual dependencies needed, see the Django docs here).

*all you must do to add your models to the admin application is to register them.*

**Registering models**

First, open admin.py in the catalog application (/locallibrary/catalog/admin.py). It currently looks like this — note that it already imports django.
This code imports the models and then calls **admin.site.register** to register each of them.

You can create a **"superuser"** account that has full access to the site and all needed permissions using manage.py.

Call the following command, in the same directory as manage.py, to create the superuser. You will be prompted to enter a username, email address, and strong password.

**>> python3 manage.py createsuperuser**

**Logging in and using the site**
To login to the site, open the /admin URL (e.g. http://127.0.0.1:8000/admin)

**Register a ModelAdmin class**
To change how a model is displayed in the admin interface you define a ModelAdmin class (which describes the layout) and register it with the model.

(Optional): [Beginner’s Guide to Django - Part 1](https://simpleisbetterthancomplex.com/series/2017/09/04/a-complete-beginners-guide-to-django-part-1.html)

## -Bookmark and Review
[Beginner’s Guide to Django - Part 2](https://simpleisbetterthancomplex.com/series/2017/09/11/a-complete-beginners-guide-to-django-part-2.html)
----

## Things I want to know more about

----
[Home](https://github.com/MISalz/401_Reading_Notes/blob/main/README.md)