# ShopHub - React.js & Tailwind CSS E-Commerce Application

A modern, responsive e-commerce application built with React.js, Tailwind CSS, and Vite. This project demonstrates component-based architecture, state management, API integration, and responsive design.

##  Live Demo

**Deployed URL:** [Add your deployment URL here]

##  Features

### Core Functionality
- ✅ **Product Catalog**: Browse all products with filtering and search
- ✅ **Product Details**: View detailed product information
- ✅ **Shopping Cart**: Add, remove, and update quantities
- ✅ **Favorites**: Mark products as favorites
- ✅ **Responsive Design**: Fully responsive across all devices
- ✅ **Routing**: Multi-page navigation with React Router

### Technical Features
- ✅ **React Hooks**: useState, useEffect, useReducer, useContext, useParams, useNavigate
- ✅ **Custom Hooks**: useFetch for API data fetching
- ✅ **Context API**: Global state management with AppContext
- ✅ **API Integration**: FakeStore API for product data
- ✅ **LocalStorage**: Persistent cart and favorites
- ✅ **Error Handling**: Comprehensive error states
- ✅ **Loading States**: Loading spinners for async operations
- ✅ **Tailwind CSS**: Modern utility-first styling

##  Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- Modern web browser
- Code editor (VS Code recommended)

## 🛠️ Installation

1. **Clone the repository**
```bash
git clone <your-repository-url>
cd <repository-name>
```

2. **Install dependencies**
```bash
npm install
```

3. **Start the development server**
```bash
npm run dev
```

4. **Open your browser**
Navigate to `http://localhost:3000`

## 📁 Project Structure

```
src/
├── api/
│   └── products.js          # API integration functions
├── components/
│   ├── Navbar.jsx           # Navigation bar component
│   ├── ProductCard.jsx      # Product card component
│   ├── LoadingSpinner.jsx   # Loading indicator
│   └── ErrorMessage.jsx     # Error display component
├── context/
│   └── AppContext.jsx       # Global state management
├── hooks/
│   └── useFetch.js          # Custom fetch hook
├── pages/
│   ├── Home.jsx             # Home page
│   ├── Products.jsx         # Products listing page
│   ├── ProductDetail.jsx    # Product detail page
│   ├── Cart.jsx             # Shopping cart page
│   ├── About.jsx            # About page
│   └── NotFound.jsx         # 404 page
├── App.jsx                  # Main application component
├── main.jsx                 # Application entry point
└── index.css                # Global styles with Tailwind
```

## 🎯 Key Components

### 1. App Component (App.jsx)
- Sets up routing with React Router
- Wraps app with AppProvider for global state
- Defines all application routes

### 2. AppContext (context/AppContext.jsx)
- Global state management using Context API
- useReducer for complex state logic
- Actions: addToCart, removeFromCart, updateQuantity, toggleFavorite
- Persists state to localStorage

### 3. Custom Hook (hooks/useFetch.js)
- Reusable data fetching logic
- Handles loading, error, and success states
- Prevents memory leaks with cleanup

### 4. API Integration (api/products.js)
- FakeStore API integration
- Functions for fetching products, categories, and product details
- Error handling for all API calls

### 5. Pages

#### Home Page
- Hero section with call-to-action
- Feature highlights
- Featured products display

#### Products Page
- Full product catalog
- Advanced filtering (category, price range, search)
- Sorting options (price, rating)
- Responsive grid layout

#### Product Detail Page
- Detailed product information
- Image display
- Add to cart with quantity selector
- Favorite toggle

#### Cart Page
- Cart items list with images
- Quantity management
- Order summary with subtotal, tax, total
- Empty cart state

## 🎨 Styling with Tailwind CSS

The application uses Tailwind CSS utility classes for styling:

- **Responsive Design**: Mobile-first approach with breakpoints
- **Custom Colors**: Extended color palette in tailwind.config.js
- **Hover Effects**: Interactive elements with hover states
- **Transitions**: Smooth animations and transitions
- **Shadows**: Depth with shadow utilities
- **Grid & Flexbox**: Modern layout techniques

## 🔄 State Management

### Global State (Context API)
```javascript
{
  cart: [],           // Shopping cart items
  favorites: [],      // Favorite product IDs
  user: null,         // User information
  theme: 'light'      // Theme preference
}
```

### Actions
- `ADD_TO_CART`: Add product to cart
- `REMOVE_FROM_CART`: Remove product from cart
- `UPDATE_QUANTITY`: Update item quantity
- `CLEAR_CART`: Clear all cart items
- `TOGGLE_FAVORITE`: Toggle favorite status
- `TOGGLE_THEME`: Switch theme
- `SET_USER`: Set user information

## 🌐 API Integration

### FakeStore API Endpoints
- `GET /products` - Fetch all products
- `GET /products/:id` - Fetch single product
- `GET /products/categories` - Fetch categories
- `GET /products/category/:category` - Fetch products by category

## 📱 Responsive Design

The application is fully responsive with breakpoints:
- **Mobile**: < 640px
- **Tablet**: 640px - 1024px
- **Desktop**: > 1024px

##  Build & Deployment

### Build for Production
```bash
npm run build
```

### Preview Production Build
```bash
npm run preview
```

### Deploy to Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Run: `vercel`
3. Follow the prompts

### Deploy to Netlify
1. Build the project: `npm run build`
2. Drag and drop the `dist` folder to Netlify
3. Or use Netlify CLI:
```bash
npm install -g netlify-cli
netlify deploy --prod
```

## 🧪 Features Demonstrated

### React Concepts
- ✅ Functional Components
- ✅ JSX Syntax
- ✅ Props and State
- ✅ Event Handling
- ✅ Conditional Rendering
- ✅ Lists and Keys
- ✅ Forms and Controlled Components
- ✅ Component Composition

### React Hooks
- ✅ useState - Local state management
- ✅ useEffect - Side effects and lifecycle
- ✅ useContext - Global state access
- ✅ useReducer - Complex state logic
- ✅ useParams - URL parameters
- ✅ useNavigate - Programmatic navigation
- ✅ Custom Hooks - Reusable logic

### Advanced Features
- ✅ React Router - Multi-page navigation
- ✅ Context API - Global state
- ✅ API Integration - External data
- ✅ LocalStorage - Data persistence
- ✅ Error Boundaries - Error handling
- ✅ Loading States - UX improvements
- ✅ Responsive Design - Mobile-first

## 📚 Technologies Used

- **React 18**: UI library
- **React Router 6**: Routing
- **Tailwind CSS 3**: Styling
- **Vite**: Build tool
- **FakeStore API**: Mock data

## 🎓 Learning Outcomes

This project demonstrates:
1. Component-based architecture
2. State management with hooks and Context API
3. API integration and data fetching
4. Responsive design with Tailwind CSS
5. Routing and navigation
6. Form handling and validation
7. Error handling and loading states
8. Performance optimization
9. Code organization and best practices

##  Known Issues

- None currently

## Future Enhancements

- [ ] User authentication
- [ ] Product reviews and ratings
- [ ] Wishlist functionality
- [ ] Order history
- [ ] Payment integration
- [ ] Dark mode
- [ ] Product comparison
- [ ] Advanced search filters
- [ ] Social sharing

## Assignment Completion Checklist

- ✅ Set up React project with Vite
- ✅ Configure Tailwind CSS
- ✅ Create reusable UI components
- ✅ Implement React Router
- ✅ Use multiple React hooks (useState, useEffect, useContext, useReducer, etc.)
- ✅ Create custom hooks
- ✅ Implement Context API for state management
- ✅ Integrate with external API
- ✅ Implement responsive design
- ✅ Handle loading and error states
- ✅ Add form handling and validation
- ✅ Implement filtering and search
- ✅ Create comprehensive documentation
- ✅ Deploy application

## 👤 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- Email: your.email@example.com

