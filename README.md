# project_2
This is a demo project.
In this project we are going to use Django RestFramework to do operation.

# operations(what to do)
=> Build a restapi for Registration/signup
=> Bulid a restapi for Login and Logout
=> Bulid a restapi for change password and reset password


# steps to setup

>first create a project and app
>create a custom user model
                  >Open models.py and define user model class
                  >And add required fields 
                  >Then open terminal and do migrations and migrate
>install djangorestframework and django-rest-knox
>add them to installed app

# steps for Registration/Signup

>Create a file in your app named 'serializers.py'
>Inside that file write your required serializer class
>Open urls.py set your path for reigstraion
>Define your class inside the views.py and write the required business logic for register
>After sucessfully register a confirmation mail will send to the mail. 

# steps for Login and Logout

>Openurls.py set a path for login and define that class inside the views.py
>Here the class inherit 'KnoxLoginView' 
> And write the required business logic for Login and Logout

# steps for change password

>Open serializers.py and creat a searializer for change password with required fiels
>Open urls.py and set the path for change password
>Define the class inside the views.py which inherit 'UpdateAPIView'
>And write the businnes logic for change password

# steps for reset password

>Install django-rest-passwordreset
> Add this to installed_app
> Open Terminal and do migrate
> Open urls.py and include django-rest-passwordreset.urls
> Open models.py and add signal for sending email
> Inside the setting.py add this (EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend')



