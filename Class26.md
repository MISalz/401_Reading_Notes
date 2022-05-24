# Class26 Reading Notes

### Readings: Intro to Django
Below you will find some reading material, code samples, and some additional resources that support today’s topic and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

### Reading
[Getting started with Django](https://www.djangoproject.com/start/)

Just the Intro to Django section.

### Object-relational mapper

A model is the single, definitive source of information about your data. It contains the essential fields and behaviors of the data you’re storing. Generally, each model maps to a single database table.

**The basics:**

1. Each model is a Python class that subclasses django.db.models.Model.
2. Each attribute of the model represents a database field.
3. With all of this, Django gives you an automatically-generated database-access API; 

**Using models**

Once you have defined your models, you need to tell Django you’re going to use those models. 

Do this by editing your settings file and changing the INSTALLED_APPS setting to add the name of the module that contains your models.py.

**Fields**

The most important part of a model – and the only required part of a model – is the list of database fields it defines. Fields are specified by class attributes. Be careful not to choose field names that conflict with the models API like clean, save, or delete.

**Relationships**

Clearly, the power of relational databases lies in relating tables to each other. Django offers ways to define the three most common types of database relationships: many-to-one, many-to-many and one-to-one.

**Models across files**

It’s perfectly OK to relate a model to one from another app. To do this, import the related model at the top of the file where your model is defined. Then, refer to the other model class wherever needed. 

[How Django Works Behind the Scenes](https://wsvincent.com/how-django-works-behind-the-scenes/)

Article explains how Django was started and funded.
  
Django’s code is open source and available to all. Django’s organization is managed by a non-profit, the DSF, with a miniscule budget. And Django code is lead by a core team of volunteers, two paid Django Fellows, and a larger group of contributors.



### Bookmark and Review
[What is Django](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Introduction)

[First Django App - Part 1](https://docs.djangoproject.com/en/3.0/intro/tutorial01/)

[First Django App - Part 2](https://docs.djangoproject.com/en/3.0/intro/tutorial02/)

----

## Things I want to know more about

----
[Home](https://github.com/MISalz/401_Reading_Notes/blob/main/README.md)