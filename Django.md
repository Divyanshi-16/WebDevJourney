# Django #
## The Web Framework for Perfectionists with Deadlines ##
- backend server side web framework
- free, open-source
- written in Python
- Once, the HTTP request has been accepted by web server, then it returns HTTP response, in the form of HTML, CSS, and JS files, but can't be interpreted by users directly. Therefore, Django converts all these files which are compatible for the users.
- Django follows MVT design pattern(Model View Template): -
  - Model: The data which is presented, usually data from the database.
           The data is delivered as an Object Relational Mapping(ORM), which makes it easier to communicate and retrieve data from the databases.
           The models are usually located in a file called models.py.
  - View: A request handler that returns the relevant template and content-based on the request from the user.
          A view is a function or method that takes http requests as arguments, imports the relevant model(s), and finds out what data to send to the template, and returns the final result.
          The views are usually located in a file called views.py.
  - Template: A text file containing the layout and design of the webpage, with logic on how to display data.
              The templates of an application is located in a folder named templates.
- URLs: Django provides a way to navigate between different web pages in a website. This is done in a file called urls.py.
- ASGI vs. WSGI
  - ASGI: - Asynchronous Server Gateway Interface
          - processes requests asynchronously
          - the processing of requests are done much faster
          - don't have to wait for other processes to finish
  - WSGI: - Web Server Gateway Interface
          - handles requests synchronously
          - when requests come in, they are processed sequentially or one after the other
          - they have to wait until the one before it finishes before switching to a new task
- Project vs. Apps
  - A project refers to the entire application and all its parts. An app refers to a submodule of the project.
  - An app is a web application that has a specific meaning in your project, like a home page, a contact form, or a members database.
### manage.py ###
    - command line utility
    - python manage.py runserver
    - python manage.py startapp home(to create a new app named home)
### Views ###
    - views are kept in the file, views.py, located on app's folder
    - these are python functions that take http requests and returns http responses.
    - create urls.py in the same folder of the app where views.py is present
    - this urls.py is then routed with the main urls.py present in the project
### Templates ###
    - stores text files (like HTML files), that defines the structure or layout of the project
### Models ###
    - to store data in the form of relational databases in models.py
