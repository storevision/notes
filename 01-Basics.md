# Basics of the application

## Discussion (18.11.2024)
- When the database + application starts, the products are initialized. (Potential extension with admin interface.)
- Database should check which schema version is there when starting (“meta” table), init + migration
- Search in the frontend (filter products -> fuse.js @CommanderRedYT)
- Send products as an array of objects to clientl
  - Properties: id, name, price_per_unit, description, inventory (count)
- Home page for anonymous users -> advertising for “Please create an account”
- When logged in
  - Shopping cart (with number in UI)
  - Shopping cart only stores list of IDs
  - “Checkout” -> Calculates total + VAT.
  - After checkout, there should be a bill / confirmation
  - After checkout, the count should be substracted from inventory
