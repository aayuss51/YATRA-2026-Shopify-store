# 🛒 YATRA – Modern E-Commerce Platform

A feature-rich, fully responsive front-end E-Commerce web application built with modern vanilla web technologies. It features dynamic product rendering, state persistence via LocalStorage, interactive shopping cart management, real-time modal search, and detailed product galleries with zoom.

🔗 **Live Demo:** right here : https://yatraecommdemo.vercel.app

---

## 🛠️ Tech Stack

### **Core Technologies**
- **HTML5**: Semantic markup, accessible page structure, and multi-page routing.
- **CSS3 (Vanilla)**: Modular CSS architecture, CSS Custom Properties (Variables), Flexbox, CSS Grid, and smooth keyframe animations.
- **JavaScript (ES6+)**: Vanilla modular JavaScript using ES Modules (`import`/`export`), asynchronous data fetching (`fetch`/`async`/`await`), and DOM manipulation.

### **Libraries & Assets**
- **[Glide.js](https://glidejs.com/)**: Fast, lightweight, dependency-free responsive slider and carousel component.
- **[Bootstrap Icons](https://icons.getbootstrap.com/)**: Clean and lightweight vector iconography.
- **[Google Fonts](https://fonts.google.com/)**: Typography powered by modern fonts (Jost / Poppins).

### **State & Data Management**
- **Browser LocalStorage API**: Persistent cart items, product state, review caching, and active product selection across page reloads.
- **JSON Data Source (`data.json`)**: Structured mock backend database for product details, pricing, discount rates, images, and reviews.

### **Deployment & Hosting**
- **Vercel**: Continuous deployment and high-performance static hosting.

---

## ✨ Core Features

### 🛍️ 1. Dynamic Product Catalog & Filtering
- **JSON-Driven Products**: Products load asynchronously from `data.json` and persist to `localStorage`.
- **Interactive Product Cards**: Dual-image hover swap (previewing secondary product angles), discount percentage badges, star ratings, and direct "Add to Cart" triggers.
- **Categorized Sections**: Featured Collections, Trending Items, New Arrivals, and Best Sellers.

### 🔍 2. Real-Time Instant Search
- **Modal Search Bar**: Quick search popup accessible from any page via the header search icon.
- **Live Filtering**: Dynamic filtering of products by title and category as the user types, with instant thumbnail, title, and price previews.

### 🛒 3. Interactive Shopping Cart System
- **State Persistence**: Cart items remain saved in `localStorage` across page navigation and browser sessions.
- **Live Cart Badge**: Header cart counter dynamically updates when items are added or removed.
- **Cart Page (`cart.html`)**:
  - Itemized table with product thumbnails, unit prices, quantities, and subtotal calculation.
  - Delete item functionality with automatic totals re-calculation.
  - **Shipping Calculator**: Toggleable fast cargo express shipping ($15.00) with automatic total adjustment.

### 🔍 4. Single Product Page Experience (`single-product.html`)
- **Product Image Gallery**: Interactive thumbnail switcher allowing users to preview multiple product angles.
- **Image Zoom**: Hover lens zoom effect on the main product image for close-up texture inspection.
- **Variant Selection**: Interactive selectors for color palettes and clothing sizes (XS, S, M, L, XL).
- **Tabbed Information System**: Seamlessly switch between **Description**, **Additional Information**, and **Reviews**.
- **Interactive Review & Rating System**: User review submission form with star rating selector and dynamic comment list insertion.

### 🎠 5. Carousels & Micro-Interactions
- **Hero Carousel (`slider.js`)**: Custom animated homepage banner slider with navigation controls and smooth fade transitions.
- **Product Carousels (`glide.js`)**: Touch-friendly multi-item sliders for showcasing featured collections and new arrivals.
- **Promotional Popup Modal**: Timed promotional newsletter discount popup that triggers automatically with overlay click-to-dismiss.

### 📱 6. Responsive & Multi-Page Layout
- **Mobile Drawer Navigation**: Slide-in hamburger menu for seamless mobile browsing.
- **8 Complete Page Templates**:
  - `index.html` – Homepage with hero banner, categories, product sliders, blogs, and newsletter.
  - `shop.html` – Full catalog view with sidebar filtering and grid layouts.
  - `single-product.html` – Comprehensive product detail page.
  - `cart.html` – Shopping cart and checkout summary.
  - `blog.html` – Blog archive grid.
  - `single-blog.html` – Detailed blog post with comment feed.
  - `account.html` – User login, registration, and account management.
  - `contact.html` – Contact form, location information, and customer support.

---

## 📁 Project Structure

```text
Ecommerce-demo-main/
├── index.html              # Homepage
├── shop.html               # Shop / Product Catalog
├── single-product.html     # Single Product Detail View
├── cart.html               # Shopping Cart Page
├── blog.html               # Blog Archive Page
├── single-blog.html        # Individual Blog Post Page
├── account.html            # User Account / Login & Register
├── contact.html            # Contact & Support Page
├── README.md               # Project Documentation
├── css/
│   ├── base.css            # CSS reset, typography, and global variables
│   ├── main.css            # Main stylesheet bundling all modules
│   ├── components/         # Modular CSS (buttons, modals, sliders, etc.)
│   ├── layout/             # Header, footer, and navigation styles
│   └── pages/              # Page-specific stylesheets
├── js/
│   ├── main.js             # Main JS entry point & initialization
│   ├── data.json           # Mock product database
│   ├── product.js          # Product rendering and routing logic
│   ├── cart.js             # Shopping cart operations & calculations
│   ├── search.js           # Search modal and real-time filter logic
│   ├── header.js           # Mobile drawer and navigation triggers
│   ├── slider.js           # Custom hero banner slider
│   ├── glide.js            # Glide.js carousel configuration
│   └── single-product/     # Single product modules (zoom, tabs, reviews, variants)
└── img/                    # Optimized image assets (products, banners, avatars)
```

---

## 🚀 Getting Started

### Prerequisites
No complex backend or build tools required! You only need a modern web browser.

### Local Installation
1. **Clone or download the repository:**
   ```bash
   git clone https://github.com/your-username/Ecommerce-demo.git
   ```
2. **Navigate to the project directory:**
   ```bash
   cd Ecommerce-demo-main/Ecommerce-demo-main
   ```
3. **Open with a local development server:**
   - **VS Code**: Right-click `index.html` and select **"Open with Live Server"**.
   - **Python (Optional)**:
     ```bash
     python -m http.server 8000
     ```
   - **Node.js (Optional)**:
     ```bash
     npx serve .
     ```
4. Open your browser and navigate to `http://localhost:8000` (or the port provided).

---

## 🌐 Live Demo

Check out the live deployment on Vercel:  
👉 https://yatraecommdemo.vercel.app

---

## 📄 License & Credits

- Developed by **Aayush Sapkota** / **Toggle Lab**.
- Built for educational and demonstration purposes.
