Backend
=======

The backend of our project is built using the Flask framework for Python.

All of the backend code is located in the `app.py` file, consisting of multiple API endpoints, including:

API List
--------

Authentication

- /api/authenticate - authenticate() - Authenticate a user using Google Firebase, crates a user account if not already exists, enables `authenticated` for access to private routes
- /api/admin/login - admin_login() - Login to an admin account using hardcoded username and password, enables `admin_authenticated` for access to admin routes
- /api/admin/logout - admin_logout() - Logout of the current admin account and move to the main homepage
- /logout - logout() - Logout of the current account and move to the main homepage

Cart

- /api/cart - POST - 
- /api/cart - GET - 
- /api/cart/add
- /api/cart/item/<int:item_id>
- /api/cart/item/<int:item_id> - DELETE -
- /api/cart/item/<int:item_id> - PUT -
- /api/cart/remove
- /api/cart/update

Chat

- /api/chat/clear-all
- /api/chat/delete/<message_id>
- /api/chat/get-customer-messages
- /api/chat/messages
- /api/chat/reply
- /api/chat/send
- /api/chat/unread-count

Dashboard

- /api/dashboard/carts
- /api/dashboard/reviews
- /api/dashboard/users

Orders

- /api/orders/place
- /api/orders/user-orders

Parts

- /api/parts/all
- /api/parts/brands
- /api/parts/search
- /api/parts/<int:part_id>

Placeholder Images

- /api/placeholder-image/<part_name>

Registrations

- /api/save_car_registration
- /api/save_part_registration

Reviews

- /account/<int:user_id>/reviews
- /api/user/reviews
- /product/<int:product_id>/review
- /product/<int:product_id>/reviews
- /product/<int:product_id>/reviews/<int:review_id>
- /seller/<int:seller_id>/review
- /api/offers

Frontend Routes

- /
- /product/{product_id}
- /search-results?q={query}
- /seller/{seller_id}
- /login
- /register
- /admin-login
- /sellers
- /account
- /cart
- /personal-details
- /car_registration
- /part_registration
- /my-orders
- /admin