# Class#33 Reading Notes

Readings: Permissions & Postgresql
Below you will find some reading material, code samples, and some additional resources that support today’s topic and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

Reading
[DRF Permissions](https://www.django-rest-framework.org/api-guide/permissions/)

Permission checks are always run at the very start of the view, before any other code is allowed to proceed. Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.

# How permissions are determined
Permissions in REST framework are always defined as a list of permission classes.

Before running the main body of the view each permission in the list is checked. If any permission check fails, an exceptions.PermissionDenied or exceptions.NotAuthenticated exception will be raised, and the main body of the view will not run.

# Object level permissions
REST framework permissions also support object-level permissioning. Object level permissions are used to determine if a user should be allowed to act on a particular object, which will typically be a model instance.

Object level permissions are run by REST framework's generic views when .get_object() is called. As with view level permissions, an exceptions.PermissionDenied exception will be raised if the user is not allowed to act on the given object.
# API Reference
AllowAny
The AllowAny permission class will allow unrestricted access, regardless of if the request was authenticated or unauthenticated.

This permission is not strictly required, since you can achieve the same result by using an empty list or tuple for the permissions setting, but you may find it useful to specify this class because it makes the intention explicit.

### IsAuthenticated
The IsAuthenticated permission class will deny permission to any unauthenticated user, and allow permission otherwise.

This permission is suitable if you want your API to only be accessible to registered users.

### IsAdminUser
The IsAdminUser permission class will deny permission to any user, unless user.is_staff is True in which case permission will be allowed.

This permission is suitable if you want your API to only be accessible to a subset of trusted administrators.

### IsAuthenticatedOrReadOnly
The IsAuthenticatedOrReadOnly will allow authenticated users to perform any request. Requests for unauthorised users will only be permitted if the request method is one of the "safe" methods; GET, HEAD or OPTIONS.

This permission is suitable if you want to your API to allow read permissions to anonymous users, and only allow write permissions to authenticated users.

### DjangoModelPermissions
This permission class ties into Django's standard django.contrib.auth model permissions. This permission must only be applied to views that have a .queryset property or get_queryset() method. Authorization will only be granted if the user is authenticated and has the relevant model permissions assigned.

POST requests require the user to have the add permission on the model.
PUT and PATCH requests require the user to have the change permission on the model.
DELETE requests require the user to have the delete permission on the model.
The default behaviour can also be overridden to support custom model permissions. For example, you might want to include a view model permission for GET requests.

To use custom model permissions, override DjangoModelPermissions and set the .perms_map property. Refer to the source code for details.

### DjangoModelPermissionsOrAnonReadOnly
Similar to DjangoModelPermissions, but also allows unauthenticated users to have read-only access to the API.

### DjangoObjectPermissions
This permission class ties into Django's standard object permissions framework that allows per-object permissions on models. In order to use this permission class, you'll also need to add a permission backend that supports object-level permissions, such as django-guardian.

As with DjangoModelPermissions, this permission must only be applied to views that have a .queryset property or .get_queryset() method. Authorization will only be granted if the user is authenticated and has the relevant per-object permissions and relevant model permissions assigned.

POST requests require the user to have the add permission on the model instance.
PUT and PATCH requests require the user to have the change permission on the model instance.
DELETE requests require the user to have the delete permission on the model instance.
Note that DjangoObjectPermissions does not require the django-guardian package, and should support other object-level backends equally well.

As with DjangoModelPermissions you can use custom model permissions by overriding DjangoObjectPermissions and setting the .perms_map property. Refer to the source code for details.

Bookmark and Review
[Classy Django REST](http://www.cdrf.co/)

[DRF Generic Views](https://www.django-rest-framework.org/api-guide/generic-views/)

----

## Things I want to know more about

----
[Home](https://github.com/MISalz/401_Reading_Notes/blob/main/README.md)