## Base Expectations

You are to build an online ordering system for a restaurant which offers both administrator and consumer interfaces.

### Unauthenticated Users

As an unauthenticated user, I can:

- [x] Browse all items
- [x] Browse items by category
- [x] Add an item to my cart
- [x] View my cart
- [x] Remove an item from my cart
- [x] Log in, which should _not_ clear the cart

Unauthenticated users are *NOT* allowed to:

- [x] View another user's private data (such as current order, etc.)
- [x] Checkout (until they log in)
- [x] View the administrator screens or use administrator functionality
- [x] Make themselves an administrator
- [x] See retired items in the menu

### Authenticated Non-Administrators

Allowed To:

- [x] do everything Unauthenticated Users can do except "log in"
- [x] log out
- [x] view their past orders with links to display each order
- [x] on that order display page there are:
  - [x] items with line-item subtotals
  - [x] links to each item description page
  - [x] the current status of the order
  - [x] order total price
  - [x] date/time order was submitted
  - [x] date/time order is ready for pickup
  - [x] if any item is retired from the menu:
     - [x] they can still access the item page
     - [x] they cannot add it to a new cart

*NOT* allowed to:

- [x] view another user's private data (such as current order, etc.)
- [x] view the administrator screens or use administrator functionality
- [x] make themselves an administrator
- [x] See retired items in the menu

### Administrators

As an authenticated Administrator, I can:

- [x] Create item listings including a name, description, price, and a photo
- [x] Modify existing items' name, description, price, and photo
- [x] Create named categories for items (eg: "Small Plates")
- [x] Assign items to categories or remove them from categories. Products can belong to one category.
- [x] Retire a item from being sold, which hides it from browsing by any non-administrator
- [x] Create savings as a percentage discount on items
- [x] Assign savings to items

As an Administrator, I can also view an order "dashboard" where I can:

- [x] See a listing of all orders with:
  - [x] the total number of orders by status
  - [x] links for each individual order
  - [x] filter orders to display by status type (for statuses "ordered", "paid", "cancelled", "completed")
  - [x] link to transition to a different status:
      - [x] link to "cancel" individual orders which are currently "ordered" or "paid"
      - [x] link to "mark as paid" orders which are "ordered"
      - [x] link to "mark as completed" individual orders which are currently "paid"
- [x] Access details of an individual order, including:
  - [x] Order date and time
  - [x] Purchaser full name and email address
  - [x] For each item on the order:
      - [x] Name with link to item page
      - [x] Price
      - [x] Line item subtotal
  - [x] Total for the order
  - [x] Status of the order
- [x] Update an individual order
  - [x] View and edit orders; remove items from orders with the status of ordered or paid
  - [x] Change the status of an order according to the rules as outlined above
