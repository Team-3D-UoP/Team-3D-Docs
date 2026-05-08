Backend
=======

The backend of our project is built using the Flask framework for Python.

All of the backend code is located in the `app.py` file, consisting of multiple API endpoints, including:

API List
--------

/api/cart
/api/user/reviews
/api/cart/add
/api/cart
/api/cart/item<int:item_id> - DELETE - 
/api/cart/item<int:item_id> - PUT - 
/api/cart/item/<int:item_id>
/api/cart/update
/api/cart/remove
/api/placeholder-image/<part_name>
/api/admin/login
/api/admin/logout
/api/dashboard/users
/api/dashboard/reviews
/api/dashboard/carts
/api/chat/send
/api/chat/messages
/api/chat/reply
/api/chat/delete/<message_id>
/api/chat/clear-all
/api/chat/get-customer-messages
/api/chat/unread-count
/api/authenticate
/api/orders/place
/api/orders/user-orders
/api/save_car_registration
/api/save_part_registration
/api/parts/all
/api/parts/search
/api/parts/<int:part_id>
/api/parts/brands
/api/offers

/seller/<int:seller_id>/review
/account/<int:user_id>/reviews
/product/<int:product_id>/review
/product/<int:product_id>/reviews
/product/<int:product_id>/reviews/<int:review_id>
/logout

/
/product/{product_id}
/search-results?q={query}
/seller/{seller_id}
/login
/register
/admin-login
/sellers
/account
/cart
/personal-details
/car_registration
/part_registration
/my-orders
/admin