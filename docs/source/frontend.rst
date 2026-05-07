Frontend
========

The frontend of our project is built using HTML, CSS and JavaScript

The frontend is split into multiple templates, including:

Public routes
-------------

Accessible to all users.

- homepage "/" - Showing the app's searching, allowing users to change cars and quickly view specific types of parts depending on usersr car's brand.

- product listing "/product/{product_id}" - Showing the product's details and allowing users to add it to usersr cart, or give a review to the user.

- search "/search-results?q={query}" - Allowing users to search for parts using a search bar, with filtering, sorting and adding to cart.

- seller profile "/seller/{seller_id}" - Showing the seller's details, including their reviews and products.

- login "/login" - Allowing users to log in to their account using google firebase or inapp.

- registration "/register" - Allowing users to register an account using google firebase or inapp.

- admin login "/admin-login" - Allowing admin users to log in to their account using inapp.

- sellers "/sellers" - Showing a list of all sellers, allowing users to easily access their profiles.

Private routes
--------------

Accessible to logged in users only.

- user account "/account" - Shows orders, personal details, user reviews.

- cart "/cart" - Showing the items in the user's cart and allowing them to update quantities or remove items and proceed to checkout.

- personal details "/personal-details" - Edit the user's username, email, name and password

- car_registration "/car_registration" - Allows users to register their car details: make, model, year produced, license plate, engine type and wheel type. 

- part_registration "/part_registration" - Allows users to register their part details: brand, year, name, price, description and type 

- my orders "/my-orders" - Showing the user's past orders.

Admin routes
------------

Accessible to admin users only.

- admin dashboard "/admin" - Showing special users: recent reviews, recent users and current chats.

Other frontend features
-----------------------

- Footer - At the bottom of each page, providing links to important pages and contact information.

- Header - At the top of each page, providing easier navigation across all pages and a search bar.

- Chat - A chat feature that allows users to communicate with sellers and support directly through the app.