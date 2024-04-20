### Project Overview

This project is an e-commerce application that allows users to view a list of furniture products and add them to a shopping cart. It utilizes JavaScript to dynamically load product data from a JSON file, manage a shopping cart, and interact with local storage to persist cart items.

### Features and Functionality

- **Initialization**
  - Fetches furniture product data from a `furniture.json` file upon page load.
  - Loads any existing cart items from local storage to display in the cart.

- **Event Listeners**
  - Listens for various user interactions such as clicking on "Add to Cart" buttons and deleting items from the cart.
  - Handles toggling visibility of the cart container and the navigation bar.

- **Product Display**
  - Dynamically generates HTML content for each product fetched from `furniture.json`.
  - Each product item includes a button to add it to the cart.

- **Cart Management**
  - Adds selected products to the cart list displayed on the UI.
  - Saves cart items to local storage for persistence across page reloads.
  - Updates cart information (total price and item count) dynamically.

- **Product Deletion**
  - Allows users to remove items from the cart by clicking on delete buttons.
  - Updates local storage and cart UI accordingly after item deletion.

### Key Components and Variables

- **DOM Elements**
  - `cartContainer`: Container for the shopping cart.
  - `productList`: Container for displaying product items.
  - `cartList`: Container for displaying items in the shopping cart.
  - `cartTotalValue`: Element displaying the total value of items in the cart.
  - `cartCountInfo`: Element displaying the count of items in the cart.
  
- **Variables**
  - `cartItemID`: Identifier used to assign unique IDs to cart items.

### How to Run

To run this project locally:

1. Ensure you have a `furniture.json` file containing furniture product data.
2. Serve the project files using a local server (e.g., `http-server` for Node.js).
3. Open the project in a web browser.
4. Interact with the product list to add items to the cart and view/update the cart.

### Notes

- The project uses `fetch` to load JSON data, so it requires a local server or live server for proper functioning due to CORS restrictions.
- Error handling is implemented to alert the user if JSON data cannot be loaded.

### Technologies Used

- **JavaScript**: For dynamic content generation, event handling, and local storage interactions.
- **HTML/CSS**: For structuring and styling the user interface.

This project provides a foundation for building a simple e-commerce frontend with basic cart functionality and local storage management. Further enhancements could include checkout processes, quantity adjustments, and more robust error handling.
