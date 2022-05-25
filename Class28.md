# Class28 Reading Notes

# Readings: Django CRUD and Forms
Below you will find some reading material, code samples, and some additional resources that support today’s topic and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

# Reading
[Django Forms](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)

An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server. Forms are a flexible mechanism for collecting user input because there are suitable widgets for entering many different types of data, including text boxes, checkboxes, radio buttons, date pickers and so on. Forms are also a relatively secure way of sharing data with the server, as they allow us to send data in POST requests with cross-site request forgery protection.

Django's form handling uses all of the same techniques that we learned about in previous tutorials (for displaying information about our models): the view gets a request, performs any actions required including reading data from the models, then generates and returns an HTML page (from a template, into which we pass a context containing the data to be displayed). What makes things more complicated is that the server also needs to be able to process data provided by the user, and redisplay the page if there are any errors.

Form
The Form class is the heart of Django's form handling system. It specifies the fields in the form, their layout, display widgets, labels, initial values, valid values, and (once validated) the error messages associated with invalid fields. 

Declaring a Form
The declaration syntax for a Form is very similar to that for declaring a Model, and shares the same field types (and some similar parameters).

Form fields
There are many other types of form fields, which you will largely recognize from their similarity to the equivalent model field classes

Validation
Django provides numerous places where you can validate your data. The easiest way to validate a single field is to override the method clean_<fieldname>() for the field you want to check.


# Bookmark and Review
[Django Templates](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Home_page)

[Django Views](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Generic_views)

----

## Things I want to know more about

----
[Home](https://github.com/MISalz/401_Reading_Notes/blob/main/README.md)