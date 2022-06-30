# Django API

- GET — The most common option, returns some data from the API based on the endpoint you visit and any parameters you provide
- POST — Creates a new record that gets appended to the database
- PUT — Looks for a record at the given URI you provide. If not, create a new record
- DELETE — Deletes the record at the given URI 
- PATCH — Update individual fields of a record
- An API is a window into a database. If you’re deploying a React application atop Django, you’ll need an API to allow React to consume information from the database.
- The Django REST Framework plays nicely with the Django ORM that’s already querying the database.
- Django allows you to define database models using Python

- Set up Django Create a model in the database that the Django ORM will manage 
- Set up the Django REST Framework Serialize the model from step 2 Create the URI endpoints to view the serialized data  
- Migrate the database whenever we create or make changes to a model, we need to tell Django to migrate those changes to the database. But Django will create a simple SQLite database for us if we don’t specify differently.
- Create a model in the database that Django ORM will manage
- The __str__ method just tells Django what to print when it needs to print out an instance of the Hero model.
- Register Hero with the admin site
- The admin site that comes out of the box with Django, it doesn’t know the Hero model exists, but with two lines of code, we can tell it about Hero.
- Create some new heroes
- Heroes API.
- Serialize the Hero model
- We need to tell REST Framework about the Hero model and how it should serialize the data.
- When a user POSTs JSON data to the API, the serializer will convert that JSON to a Hero model for us to save or validate.
- Import the Hero model
- Import the REST Framework serializer 
-Create a new class that links the Hero with its serializer 
- Query the database for all heroes 
- Pass that database queryset into the serializer we just created so that it gets converted into JSON and rendered ModelViewSet is a special view that Django Rest Framework provides.
1. Set up Django
- 1.1 Virtual Environment
- 1.2 Install Django
- 1.3 Create API app
- 1.4 Register the myapi app with the mysite project
- 1.5 Migrate the database
- 1.6 Create Super User
2. Create a model in the database that Django ORM will manage
- 2.1 myapi/models.py
- 2.2 Make migrations
- 2.3 Register Hero with the admin site
- 2.4 Create some new heroes
3. Set up Django REST Framework
4. Serialize the Hero model
5. Display the data
- 5.1 Views
- 5.2 Site URLs
- 5.3 API URLs

