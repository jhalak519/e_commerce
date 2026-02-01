# About The Project

This is a Django-based e-commerce application designed to provide a complete online shopping experience. Users can register, log in, browse products by category, filter by price, add items to their cart, and place orders. The admin panel allows for easy management of products and orders.

## Features

### User Authentication
*   User registration with username and password.
*   Secure login and logout functionality.
*   Customer profile creation with address details (name, address, city, state, pin code, mobile number).

### Product Browsing
*   Homepage showcasing featured, latest, and offer products.
*   Dedicated pages for Men, Women, and Kids categories.
*   Product detail view with descriptions, pricing, available colors, and sizes.

### Price Filtering
*   Filter products by price range:
    *   Price 100-500
    *   Price 500-1000
    *   Price Over 1000

### Shopping Cart
*   Add products to cart from the product detail page.
*   View all items in the shopping cart.
*   Remove items from the cart.
*   See subtotal, tax, and total amount.

### Buy Now
*   Quick purchase option that adds the product to the cart and redirects directly to checkout.

### Checkout and Orders
*   Checkout page to review items and select delivery address.
*   Order confirmation and payment completion flow.
*   View order history with details of past purchases.

### Site Information
*   About Us modal with information about the store.
*   Contact Us modal with phone, email, and social media details.

---

## Project Structure

The project is organized into several Django applications:

```
e_commerce/
|-- authenticationapp/   # Handles user registration, login, logout, and customer profiles
|-- dashboradapp/        # Dashboard related functionality
|-- e_commerce/          # Main project settings and URL configuration
|-- mainapp/             # Core app for landing page elements
|-- productapp/          # Products, categories, cart, checkout, and order management
|-- media/               # Uploaded product images
|-- static/              # Static files (CSS, JS, images)
|-- templates/           # HTML templates for all apps
|-- db.sqlite3           # SQLite database file
|-- manage.py            # Django management script
|-- requirements.txt     # Python dependencies
```

---

## Technology Stack

*   **Backend Framework:** Django 5.x
*   **Programming Language:** Python 3.13
*   **Frontend:** HTML5, CSS3, JavaScript
*   **CSS Framework:** Bootstrap 5
*   **Icons:** Font Awesome
*   **Database:** SQLite (default, can be configured for PostgreSQL or MySQL)

---

## Getting Started

Follow these steps to set up the project on your local machine.

### Prerequisites

*   Python 3.10 or higher
*   pip (Python package installer)
*   Virtual environment (recommended)

### Installation

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd e_commerce
    ```

2.  **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3.  **Install the required packages:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Apply database migrations:**
    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

5.  **Create a superuser for admin access (optional):**
    ```bash
    python manage.py createsuperuser
    ```

6.  **Run the development server:**
    ```bash
    python manage.py runserver
    ```

7.  **Access the application:**
    Open your browser and go to `http://127.0.0.1:8000/`

---

## Usage

*   **Home Page:** Browse featured, latest, and offer products.
*   **Category Pages:** Navigate to Men, Women, or Kids sections to see relevant products. Use price filters to narrow down results.
*   **Product Details:** Click on any product to see its full details, colors, and sizes. Add to cart or buy now.
*   **Cart:** Review your selected items, see totals, and proceed to checkout.
*   **Checkout:** Confirm your order and complete the purchase.
*   **Account:** Register or log in to manage your profile and view order history. Click on the user icon to access profile, logout, and orders.
*   **Admin Panel:** Visit `/admin/` and log in with superuser credentials to manage products, users, and orders.

---

## Contact

For questions or support, please use the Contact Us section within the application or reach out via:

*   **Phone:** 1234567890
*   **Email:** shop@email.com
*   **Instagram:** shop.us
*   **LinkedIn:** shopus.in
*   **Twitter:** shopusnow
