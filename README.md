# EcoCart Smart Swap 🌱

A modern, eco-friendly e-commerce platform that promotes sustainable shopping by suggesting environmentally friendly alternatives to traditional products.

## Tech Stack

### Frontend
- **React** with TypeScript
- **Vite** for fast development
- **Tailwind CSS** for styling
- **Radix UI** for components
- **Auth0** for authentication
- **React Router** for navigation

### Backend
- **Node.js** with Express
- **MongoDB** with Mongoose
- **JWT** for authentication
- **CORS** for cross-origin requests
- **Auth0** integration

## Getting Started

### Prerequisites
- Node.js (v16 or higher)
- MongoDB Atlas account
- Auth0 account

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/eco-cart-smart-swap.git
   cd eco-cart-smart-swap
   ```

2. **Setup Backend**
   ```bash
   cd backend
   npm install
   ```

3. **Setup Frontend**
   ```bash
   cd frontend
   npm install
   ```

### Environment Configuration

#### Backend (.env)
```properties
MONGO_URI=mongodb+srv://aarnavanand5:aarnav@cluster0.nipmnyj.mongodb.net/
AUTH0_DOMAIN=dev-dji23lgbbvgw80ol.us.auth0.com
AUTH0_AUDIENCE=https://dev-dji23lgbbvgw80ol.us.auth0.com/api/v2/
```

#### Frontend (.env)
```properties
VITE_AUTH0_DOMAIN=dev-dji23lgbbvgw80ol.us.auth0.com
VITE_AUTH0_CLIENT_ID=vMHHnwpbhBPDaehdMmblzfvcAHtD5WDl
VITE_AUTH0_AUDIENCE=https://dev-dji23lgbbvgw80ol.us.auth0.com/api/v2/
VITE_API_URL=http://localhost:5000/api
```

### Auth0 Configuration

1. **Create Auth0 Application**
   - Go to [Auth0 Dashboard](https://manage.auth0.com/)
   - Create a new Single Page Application
   - Configure callback URLs: `http://localhost:5173`, `http://localhost:3000`

2. **Create Auth0 API**
   - Create a new API with identifier: `https://your-domain.us.auth0.com/api/v2/`
   - Use RS256 signing algorithm

### Running the Application

1. **Start Backend**
   ```bash
   cd backend
   npm start
   ```
   Backend will run on `http://localhost:5000`

2. **Start Frontend**
   ```bash
   cd frontend
   npm run dev
   ```
   Frontend will run on `http://localhost:5173`

## Project Structure

```
eco-cart-smart-swap/
├── backend/
│   ├── config/
│   │   └── db.js
│   ├── controllers/
│   │   ├── authController.js
│   │   ├── cartController.js
│   │   ├── productController.js
│   │   └── userController.js
│   ├── middleware/
│   │   ├── authMiddleware.js
│   │   └── errorHandler.js
│   ├── models/
│   │   ├── User.js
│   │   ├── Product.js
│   │   └── Cart.js
│   ├── routes/
│   │   ├── authRoutes.js
│   │   ├── cartRoutes.js
│   │   └── productRoutes.js
│   ├── utils/
│   │   └── ecoUtils.js
│   └── server.js
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── auth/
│   │   │   ├── customer/
│   │   │   ├── admin/
│   │   │   └── ui/
│   │   ├── hooks/
│   │   ├── services/
│   │   ├── types/
│   │   └── pages/
│   ├── public/
│   └── package.json
└── README.md
```

## API Endpoints

### Authentication
- `POST /api/auth/login` - User login
- `POST /api/auth/register` - User registration
- `GET /api/auth/me` - Get current user

### Products
- `GET /api/products` - Get all products
- `GET /api/products/:id` - Get product by ID
- `POST /api/products` - Create product (Admin only)
- `PUT /api/products/:id` - Update product (Admin only)
- `DELETE /api/products/:id` - Delete product (Admin only)

### Cart
- `GET /api/cart` - Get user's cart
- `POST /api/cart/add` - Add item to cart
- `PUT /api/cart/update` - Update cart item
- `DELETE /api/cart/remove` - Remove item from cart

### Analytics
- `GET /api/analytics/dashboard` - Get dashboard data
- `GET /api/analytics/eco-impact` - Get environmental impact data

## User Roles

### Customer
- Browse products
- Add items to cart
- View eco-friendly alternatives
- Track environmental impact
- Access personal dashboard

### Admin
- Manage products (CRUD operations)
- View analytics dashboard
- Manage users
- Monitor system performance

## Deployment

### Frontend (Vercel)
```bash
npm install -g vercel
vercel login
cd frontend
vercel
```

### Backend (Render/Railway)
1. Create account on deployment platform
2. Connect GitHub repository
3. Set environment variables
4. Deploy

### Environment Variables for Production
- Update Auth0 callback URLs
- Set production API URLs
- Configure CORS origins

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support
For support, email support@ecocart.com or join our Slack channel.

## Acknowledgments

- Auth0 for authentication services
- MongoDB for database hosting
- Vercel for frontend hosting
- All contributors who helped build this project

---

![Screenshot (67)](https://github.com/user-attachments/assets/3226eac0-e364-4937-91ea-a5ffe3414db1)

A real-time React-based web app that recommends greener, more sustainable product alternatives while you shop — reducing cart emissions by up to 40%.
![Screenshot (68)](https://github.com/user-attachments/assets/add258a9-55b7-4cad-8a62-818134a80f2e)


🚀 Features
♻️ Eco-Score Tags: Highlights each product's sustainability score
🛒 Green Cart System: Helps track the total environmental impact of your cart
📉 CO₂ Savings Dashboard: Visualizes how much carbon footprint you're saving
🔍 Real-Time Product Search with intelligent green filtering
🔐 Custom Auth System for user logins and tracking behavior
🏆 Leaderboard: Monthly leaderboard showing the top eco-friendly shoppers
🔄 Live Updates with Convex’s real-time backend

![Screenshot (70)](https://github.com/user-attachments/assets/c7aeb141-461d-48c6-bb26-91d88e597f49)
![Screenshot (69)](https://github.com/user-attachments/assets/bafd633d-59b5-441e-b7d4-e906fe58fee2)



🛠 Tech Stack
Frontend: React.js, Tailwind CSS, JavaScript
Backend & DB: Convex (zero-config backend with live queries)
UX: React Hot Toast (notifications)

👥 Users
Engaged 50+ test users, tracked usage patterns, and collected insights for future improvements in sustainable shopping habits.

![Screenshot (70)](https://github.com/user-attachments/assets/df1a9530-a138-4225-b186-139e2dcf2c63)


**Made with ❤️ for a sustainable future** 🌍
