How we implemented the project
==============================

User Types
----------

Our projects has two types of users: customers and admins. Customers are able to register cars, car parts and purchase car parts, as well as leave reviews and contact support. Admins provide support to customers, and have access to a dashboard showing user statistics, as well as reply to customer's messages.

Three-Layered Application
-------------------------

Our project is a three-layered application, consisting of a frontend, backend and multiple databases:

Frontend
--------

HTML, CSS and JavaScript

Split into multiple templates, including: a main home page, registration pages, user authentication pages, and a search page.

Backend
-------

Flask framework for Python

Split into multiple functions, including: routing, database interaction, and API endpoints.

Databases
---------

- Firebase for user authentication and storing chats - chosen for its increased security and ease of use
- SQLalchemy for storing reviews - chosen for its quick creation and ease of use
- SQLite for storing car parts and cars - chosen for its simplicity and suitability for the application's needs

Three databases were used so that we could develop multiple parts of the project concurrently.