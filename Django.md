# Django #
## The Web Framework for Perfectionists with Deadlines ##
- backend server side web framework
- free, open-source
- written in Python
- Django follows MVT design pattern(Model View Template): -
  - Model: The data which is presented, usually data from the database.
           The data is delivered as an Object Relational Mapping(ORM), which makes it easier to communicate and retrieve data from the databases.
           The models are usually located in a file called models.py.
  - View: A request handler that returns the relevant template and content-based on the request from the user.
          A view is a function or method that takes http requesta as arguments, imports the relevant model(s), and finds out what data to send to the template, and returns the final result.
          The views are usually located in a file called views.py.
  - Template: A text file containing the layout and design of the webpage, with logic on how to display data.
              The templates of an application is located in a folder named templates.
- URLs: Django provides a way to navigate between different web pages in a website. This is done in a file called urls.py.
