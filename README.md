# e-plantShopping

**e-plantShopping** is the repository for **Paradise Nursery**, an online plant shop built with React and Redux Toolkit. Visitors land on a welcome page, browse houseplants by category, add plants to a shopping cart, and manage their cart before checkout.

## Overview

Paradise Nursery ("Where Green Meets Serenity") is a single-page shopping app for plant lovers. It shows how to build a small e-commerce front end with reusable React components and a central Redux store that keeps the cart in sync across the whole app.

## Features

- **Landing page:** a welcome screen with a background image, a short "About Us" section, and a **Get Started** button that opens the store.
- **Product listing:** plants grouped into five categories:
  - Air Purifying Plants
  - Aromatic Fragrant Plants
  - Insect Repellent Plants
  - Medicinal Plants
  - Low Maintenance Plants

  Each plant shows an image, a name, a short description, and a price.
- **Add to cart:** each plant has an **Add to Cart** button, and the cart icon in the navbar shows how many items are in the cart.
- **Shopping cart page:**
  - Increase or decrease the quantity of each plant
  - Remove plants from the cart
  - See the subtotal for each item and the total for the whole cart
  - **Continue Shopping** to go back to the product list, or **Checkout**
- **Navigation:** a navbar with links to Home, Plants, and Cart.

## Tech Stack

- [React 18](https://react.dev/) for the UI components
- [Redux Toolkit](https://redux-toolkit.js.org/) and [React Redux](https://react-redux.js.org/) for cart state management
- [Vite](https://vitejs.dev/) for the dev server and build tool
- [gh-pages](https://github.com/tschaub/gh-pages) for deployment to GitHub Pages

## Project Structure

```
src/
├── App.jsx          # Landing page and switching between landing page and store
├── AboutUs.jsx      # About Us section shown on the landing page
├── ProductList.jsx  # Navbar and plant catalog grouped by category
├── CartItem.jsx     # Shopping cart page (quantities, totals, checkout)
├── CartSlice.jsx    # Redux slice: addItem, removeItem, updateQuantity
├── store.js         # Redux store configuration
└── main.jsx         # App entry point, wraps App in the Redux Provider
```

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (version 18 or later recommended)
- npm

### Installation

```bash
git clone https://github.com/gvaughn3/e-plantShopping.git
cd e-plantShopping
npm install
```

### Run locally

```bash
npm run dev
```

Then open the local URL that Vite prints in the terminal.

### Build for production

```bash
npm run build
npm run preview
```

## License

This project is licensed under the terms of the [LICENSE](LICENSE) file in this repository.
