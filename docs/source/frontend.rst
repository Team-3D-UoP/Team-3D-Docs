Frontend
========

The frontend of our project is built using HTML, CSS and JavaScript

The frontend is split into multiple templates, including:

Public routes
-------------

Accessible to all users.

- homepage "/"
- product listing "/product/{product_id}"
- search "/search-results?q={query}"
- seller profile "/seller/{seller_id}"
- seller reviews "/seller/{seller_id}/review"
- login "/login"
- registration "/register"
- admin login "/admin-login"
- sellers "/sellers"

Private routes
--------------

Accessible to logged in users only.

- user account "/account"
- cart "/cart"
- personal details "/personal-details"
- car_registration "/car_registration"
- part_registration "/part_registration"
- my orders "/my-orders"

Admin routes
------------

Accessible to admin users only.

- admin dashboard "/admin"

Other frontend features
-----------------------

- Footer - At the bottom of each page, providing links to important pages and contact information.
- Header - At the top of each page, providing easier navigation across all pages and a search bar.
- Chat - A chat feature that allows users to communicate with sellers and support directly through the app.