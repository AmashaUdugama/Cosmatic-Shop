# 💄 Cosmetic Shop

A modern e-commerce platform for beauty and cosmetic products built with React and Node.js.

## ✨ Features

- 🛍️ Product catalog with search and filtering
- 🔐 User authentication and profiles
- 🛒 Shopping cart and checkout
- 📦 Order management
- 👨‍💼 Admin dashboard
- 📱 Responsive design

## 📋 Prerequisites

- 🟢 Node.js (v14+)
- 🍃 MongoDB
- 📦 npm or yarn

## 🚀 Installation

1. **Clone the repository**
```bash
git clone https://github.com/AmashaUdugama/Cosmatic-Shop.git
cd Cosmatic-Shop
```

2. **Install dependencies**
```bash
npm install
```

3. **Create `.env` file**
```env
MONGODB_URI=mongodb://localhost:27017/cosmetic_shop
JWT_SECRET=your_jwt_secret
PORT=3000
```

4. **Start the application**
```bash
npm start
```

🌐 Visit `http://localhost:3000`

## 🛠️ Tech Stack

**Frontend:** ⚛️ React, 🌐 HTML5, 🎨 CSS3, 📜 JavaScript  
**Backend:** 🟢 Node.js, ⚡ Express.js  
**Database:** 🍃 MongoDB, 📊 Mongoose  
**Authentication:** 🔑 JWT

## 📁 Project Structure

```
src/
├── 🧩 components/     # React components
├── 📄 pages/         # Application pages
├── 🔧 services/      # API services
├── 🛠️ utils/         # Helper functions
└── 🎨 styles/        # Stylesheets
```

## 🔗 API Endpoints

### 🔐 Authentication
- `POST /api/auth/register` - Register user
- `POST /api/auth/login` - Login user

### 🛍️ Products
- `GET /api/products` - Get all products
- `GET /api/products/:id` - Get single product
- `POST /api/products` - Create product (Admin)

### 🛒 Cart & Orders
- `POST /api/cart/add` - Add to cart
- `GET /api/orders` - Get user orders
- `POST /api/orders` - Create order

## 🤝 Contributing

1. 🍴 Fork the repository
2. 🌿 Create feature branch (`git checkout -b feature/amazing-feature`)
3. 💾 Commit changes (`git commit -m 'Add amazing feature'`)
4. 📤 Push to branch (`git push origin feature/amazing-feature`)
5. 🔄 Open Pull Request

## 📄 License

📜 MIT License - see [LICENSE](LICENSE) file for details.

---

⭐ **Star this repo if you find it helpful!** ⭐
