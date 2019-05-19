# IT Tasks

The task list for the upcoming two sprints

 ### Key Notes:
 
 * Make sure to follow DRY principle (Don't Repeat Yourself). If you feel that a part of the code is reusable, encapsulate it to reuse it instead of rewriting it over and over. This provides a simple, easy to read, and clean code.
 * Make sure to use GitHub, commit your work every now and then so you can go back to a previous step when necessary.
   * Use a new branch for every module or feature or section you're adding to the project, to keep the master branch clean and easy to maintain.

# Back-end

   (These are not small tasks but most upcoming tasks will be adding features or modules like this)

### Django - Dashboard

#### Instructions:

  * Make sure no one can enter and browse the dashboard unless he/she is signed in.
  * Use Bootstrap for rapid styling as we go

#### Tasks:

  1. Market Module (Views and CRUD functionality)
     * Index page (main page that lists all Markets)
     * Create page (form to create a new market)
       * save function (to save the record in the database)
     * Show page (shows the details of one market)
     * Edit page (form to edit the fields of a market)
       * update function (to apply changes from edit form)
     * Delete function (deletes the record from the database)
  
  2. Store Module (Views and CRUD functionality)
     * Index page (main page that lists all supermarket branches)
     * Create page (form to create a new branch of a market)
       * save function (to save the record in the database)
     * Show page (shows the details of one branch)
     * Edit page (form to edit the fields of a branch)
       * update function (to apply changes from edit form)
     * Delete function (deletes the record from the database)

  3. Category Module (Views and CRUD functionality)
     * Index page (main page that lists all categories)
     * Create page (form to create a new category)
       * save function (to save the record in the database)
     * Show page (shows the details of one category)
     * Edit page (form to edit the fields of a category)
       * update function (to apply changes from edit form)
     * Delete function (deletes the record from the database)

  4. Users Module (Views)
     * Index page (main page that lists all users)
     * Show page (shows the details of a single user)
     * Edit page (form to change and configure a user)
       * update function (to apply changes from edit form)

  5. Product Module (Views and CRUD functionality)
     * Index page (main page that lists all products)
     * Create page (form to create a new product)
       * save function (to save the record in the database)
     * Show page (shows the details of one product)
     * Edit page (form to edit the fields of a product)
       * update function (to apply changes from edit form)
     * Delete function (deletes the record from the database)


### Django - API

#### Instructions:

  * Make sure to validate every request's headers and parameters (body).
  * In every response, make sure to provide necessary information like Status Code (200, 401, 500 ... etc.) and Success (true or false).
  * Besides the allowed pages (browsing products for example), make sure to authenticate the user on every route.
  * Use Postman to test your work and save the requests you're creating for future references.
  * Be aware that in the future we will use pagination (limited collection per page)

#### Tasks:

  1. Main page
     * Create the route (url)
     * Validate the request in the view
     * Send a response with the main page content (categories and products)


  2. Login/Logout
     * Create the route (url)
     * Validate the request AND authenticate the user
     * Send a response with the successful message and token

  3. Categories (and single category)
     * Create the routes
     * Validate the request
     * Respond with (all categories OR a category)

  4. Products (and single product)
     * Create the routes
     * Validate the request
     * Respond with (all products OR a product) needed
       * Handle filtration if provided with the route (example: api/products?category="Food" this route should return all products of category Food)

  5. User Profile (both to view and update)
     * Create the routes
     * Validate the request
     * Respond with the user's information
     * Handle updating user's profile

---

# Front-end

#### Instructions:

  * Use Angular Material for easy development and to make the web app look responsive, pretty, and clean. (Angular material is a library that provides pre-made customized components the follows Google's material design philosophy)
  * Make sure to structure the project properly, you will need to make folder for each component and folder to hold shared components, and different folders to hold logic scripts such as Services and Guards
  * Try reusing components as much as possible
  * Divide each segment, part, or section into component. Then divide that component into further smaller components.

#### Tasks:

  1. Create the Navbar component
     * Holds the Logo
     * Holds navigation menu list
     * Represents the cart

  2. Create the main page
     * Composed of the following parts:
       * Search
       * Filter
       * Sections for each category and their products

  3. Create Category page
     * Composed of the following parts:
       * Category title
       * Search
       * Filter
       * List of products in that category

  4. Create Product page
     * Composed of the following parts:
       * Product Image
       * Product Details
       * Action buttons (Add to cart, +/- buttons, quantity)

  5. Create Cart page
     * Composed of the following parts:
       * Cart title and total price
       * List of products in the cart
       * Calculated price (with vat and offers)
       * Action buttons (Checkout, or Save cart, or Submit)

  6. Loading spinner (to be discussed later)


---

# Data Analysis


#### Instructions:

  * Document you're steps and save you're references that helped you finish your work.
  * Please use Qaren's official email for any tool to be used that requires login or creating new account.
  * I you have apps or codes locally in you're machine please let us know to create a repository for you to upload and share your work.

#### Tasks:

  1. Prepare an updatable spreadsheets (Urgent)
     * Spreadsheet for each market that holds the Name, Price, and Image
     * Can be scrapped and updated easily for regular uses
     * Can be used for the Marketing Tool

  2. Unite product names
     * Prepare the system to unite all different products within one name (the desired name can be changed and the system should still work)
     * Make sure it is scalable, we will be adding more products in the future.
     * Make it work with the current Qaren website and compatible or adjustable to work with the new website.

  3. Exporting filtration
     * Figure out a way to extract the scripts and tools that runs the filtration process so that we can implement it in our system and make it an automated process. 

  4. Prepare a strategy to study user interaction
     * Create a strategy that we can implement in our back-end system to track and log user interaction. To get better understanding of our target customers and improve our services.