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

- /api/cart - POST - add_product_to_cart() - adds an item to the cart, with id, name, price and quantity (For non-authenticated users)
- /api/cart - GET - get_cart() - retrieves all items in the user's cart
- /api/cart/add - add_to_cart() - adds an item to the cart, aswell as to the firebase DB for persistent storage (For authenticated users)
- /api/cart/item/<int:item_id> - DELETE - remove_from_cart(item_id) - removes an item from the cart depending on the item_id
- /api/cart/item/<int:item_id> - PUT - update_cart_item(item_id) - updates the quantity of an item in the cart depending on the item_id and post quantity
- /api/cart/remove - remove_cart_item() - removes an item from the cart, depending on the JSON data
- /api/cart/update - update_cart_quantity() - updates the quantity of an item in the cart using increments

Chat

- /api/chat/clear-all - clear_all_chats() - Clears all chats from the firebase database (`admin_authenticated` only)
- /api/chat/delete/<message_id> - delete_chat_message(message_id) - Deletes a single chat with message_id from the firebase database (`admin_authenticated` only)
- /api/chat/get-customer-messages - get_customer_messages() - Gets chat messages from the firebase database, showing all results if `admin_authenticated` is true, or only chats with the correct email if false
- /api/chat/messages - get_chat_messages() - Admin only route to get all chat messages from the firebase database (`admin_authenticated` only)
- /api/chat/reply - reply_to_chat() - Route for an admin to reply to a chat message using the firebase database (`admin_authenticated` only)
- /api/chat/send - send_chat_message() - Route for a user to send a chat message using the firebase database
- /api/chat/unread-count - unread_chat_count() - Gets the count of unread chat messages for an admin from the firebase database (`admin_authenticated` only)

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