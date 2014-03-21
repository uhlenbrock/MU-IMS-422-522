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
- [ ] Checkout (until they log in)
- [x] View the administrator screens or use administrator functionality
- [x] Make themselves an administrator
- [ ] See retired items in the menu

### Authenticated Non-Administrators

Allowed To:

- [x] do everything Unauthenticated Users can do except "log in"
- [x] log out
- [ ] view their past orders with links to display each order
- [ ] on that order display page there are:
  - [ ] items with line-item subtotals
  - [ ] links to each item description page
  - [ ] the current status of the order
  - [ ] order total price
  - [ ] date/time order was submitted
  - [ ] if any item is retired from the menu:
     - [ ] they can still access the item page
     - [ ] they cannot add it to a new cart

*NOT* allowed to:

- [x] view another user's private data (such as current order, etc.)
- [x] view the administrator screens or use administrator functionality
- [x] make themselves an administrator
- [ ] See retired items in the menu

### Administrators

As an authenticated Administrator, I can:

- [x] Create item listings including a name, description, price, and a photo
- [x] Modify existing items' name, description, price, and photo
- [x] Create named categories for items (eg: "Small Plates")
- [x] Assign items to categories or remove them from categories. Products can belong to one category.
- [ ] Retire a item from being sold, which hides it from browsing by any non-administrator

As an Administrator, I can also view an order "dashboard" where I can:

- [ ] See a listing of all orders with:
  - [ ] the total number of orders by status
  - [ ] links for each individual order
  - [ ] filter orders to display by status type (for statuses "ordered", "paid", "cancelled", "completed")
  - [ ] link to transition to a different status:
      - [ ] link to "cancel" individual orders which are currently "ordered" or "paid"
      - [ ] link to "mark as paid" orders which are "ordered"
      - [ ] link to "mark as completed" individual orders which are currently "paid"
- [ ] Access details of an individual order, including:
  - [ ] Order date and time
  - [ ] Purchaser full name and email address
  - [ ] For each item on the order:
      - [ ] Name with link to item page
      - [ ] Price
      - [ ] Line item subtotal
  - [ ] Total for the order
  - [ ] Status of the order
- [ ] Update an individual order
  - [ ] View and edit orders; remove items from orders with the status of pending or paid
  - [ ] Change the status of an order according to the rules as outlined above
