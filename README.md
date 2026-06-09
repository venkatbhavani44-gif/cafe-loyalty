# Cafe Loyalty & Pre-Order Platform

A full-stack, responsive, and progressive web application for a modern cafe business. This platform enables customers to earn loyalty points, pre-order items, and make payments seamlessly while providing cafe owners with comprehensive management and analytics tools.

## 🚀 Features

### Customer Features
- ✅ User Registration & Login with JWT Authentication
- ✅ Digital Loyalty Card with QR Code Tracking
- ✅ Earn Points on Every Purchase
- ✅ Reward Redemption System
- ✅ Browse & Pre-Order Menu Items
- ✅ Razorpay Payment Integration
- ✅ Real-time Order Tracking
- ✅ Push & Email Notifications
- ✅ Mobile Responsive Design
- ✅ PWA with Offline Support
- ✅ Dark/Light Theme Toggle

### Admin Dashboard
- ✅ Customer Management
- ✅ Loyalty Points Management
- ✅ Rewards Management
- ✅ Menu Items Management
- ✅ Order Management
- ✅ Event Management
- ✅ Analytics & Revenue Reports
- ✅ Customer Insights

### Cafe Website
- ✅ Modern Coffee-Themed Design
- ✅ Virtual Cafe Tour Gallery
- ✅ Customer Testimonials
- ✅ Event Listings (Open Mic, Live Music, Art Exhibitions)
- ✅ Private Event Booking
- ✅ Contact Form

## 📋 Tech Stack

- **Frontend**: React.js, Tailwind CSS, Redux Toolkit
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Tokens)
- **Payment**: Razorpay
- **Notifications**: Push Notifications, SendGrid (Email)
- **PWA**: Workbox, Service Workers
- **Deployment**: Docker, AWS/Heroku Ready

## 📁 Project Structure

```
cafe-loyalty/
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── redux/
│   │   ├── utils/
│   │   ├── styles/
│   │   ├── App.jsx
│   │   └── index.jsx
│   ├── package.json
│   └── tailwind.config.js
├── backend/
│   ├── models/
│   ├── routes/
│   ├── controllers/
│   ├── middleware/
│   ├── utils/
│   ├── config/
│   ├── server.js
│   └── package.json
├── docs/
│   ├── API.md
│   ├── DATABASE.md
│   └── DEPLOYMENT.md
├── docker-compose.yml
├── .env.example
└── README.md
```

## 🔧 Installation & Setup

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (Local or Atlas)
- npm or yarn

### Backend Setup

```bash
cd backend
npm install

# Create .env file
cp .env.example .env

# Configure environment variables
# MONGODB_URI=your_mongodb_connection_string
# JWT_SECRET=your_jwt_secret_key
# RAZORPAY_KEY_ID=your_razorpay_key
# RAZORPAY_KEY_SECRET=your_razorpay_secret
# SENDGRID_API_KEY=your_sendgrid_key

# Start the server
npm start
```

### Frontend Setup

```bash
cd frontend
npm install

# Create .env.local file
cp .env.example .env.local

# Configure environment variables
# REACT_APP_API_URL=http://localhost:5000

# Start the development server
npm start
```

## 📚 API Documentation

See [API.md](./docs/API.md) for complete API documentation.

### Key Endpoints

**Authentication**
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user
- `POST /api/auth/refresh` - Refresh JWT token

**Customers**
- `GET /api/customers/profile` - Get user profile
- `PUT /api/customers/profile` - Update profile
- `GET /api/customers/loyalty` - Get loyalty points
- `GET /api/customers/rewards` - Get available rewards

**Orders**
- `POST /api/orders` - Create order
- `GET /api/orders` - Get user orders
- `GET /api/orders/:id` - Get order details
- `PUT /api/orders/:id/status` - Update order status

**Menu**
- `GET /api/menu` - Get all menu items
- `GET /api/menu/:id` - Get menu item details

**Payments**
- `POST /api/payments/razorpay` - Create Razorpay order
- `POST /api/payments/verify` - Verify payment

## 🗄️ Database Schema

See [DATABASE.md](./docs/DATABASE.md) for detailed MongoDB collections schema.

### Collections
- **Users** - Customer information, authentication
- **Orders** - Order details and history
- **MenuItems** - Cafe menu with categories
- **Rewards** - Loyalty rewards catalog
- **Events** - Cafe events and bookings
- **Bookings** - Private event reservations
- **Notifications** - Push and email notifications

## 🔐 Security Features

- JWT-based authentication
- Password hashing with bcrypt
- CORS protection
- Rate limiting
- Input validation and sanitization
- HTTPS ready
- Secure payment processing

## 📱 PWA Features

- **Offline Support**: Service workers cache essential data
- **Install Prompt**: Users can install as app
- **Push Notifications**: Real-time order updates
- **Fast Loading**: Optimized assets and caching strategies
- **App Shell Architecture**: Quick load times

## 🚀 Deployment

### Docker Deployment

```bash
docker-compose up -d
```

### Heroku Deployment

```bash
# Backend
heroku create cafe-loyalty-api
git push heroku main

# Frontend
npm run build
# Deploy to Vercel or Netlify
```

See [DEPLOYMENT.md](./docs/DEPLOYMENT.md) for detailed instructions.

## 📊 Admin Dashboard

Access admin panel at `/admin/dashboard` with admin credentials.

**Features:**
- Real-time analytics
- Revenue tracking
- Customer insights
- Inventory management
- Event scheduling
- Order fulfillment tracking

## 🎨 UI/UX Features

- Modern minimalist design
- Warm earth-tone color palette
- Smooth animations and transitions
- Fully responsive (Mobile, Tablet, Desktop)
- Dark and Light theme support
- Accessibility (WCAG 2.1 AA)

## 📞 Support & Contact

For support, please contact: support@cafeloyalty.com

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Author

Developed with ❤️ for modern cafes.

---

**Version:** 1.0.0  
**Last Updated:** June 2026
