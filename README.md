

# 🌍 **Wanderlust – Holiday Rental Website**

A full-stack holiday rental web application built using **Node.js, Express, MongoDB, EJS, Cloudinary**, and secured with **JWT authentication**.

---

## 📌 **Overview**

**Wanderlust** is a dynamic **holiday rental platform** where users can browse properties, view detailed information, and manage listings. The platform provides secure login/signup, property management, image uploads, and a smooth user experience using server-side rendered EJS pages. Images are handled through **Cloudinary**, while **MongoDB** stores all backend data such as users and listings. The entire backend is written in **Express**, ensuring fast API responses and secure routing controlled by JWT & bcrypt.js.

---

## 🚀 **Live Demo**

🔗 **Frontend/Website:** [https://wanderlust-kbq6.onrender.com](https://wanderlust-kbq6.onrender.com)

🔗 **GitHub Repository:** [https://github.com/ashish117840/Wanderlust](https://github.com/ashish117840/Wanderlust)

---

## 🛠️ **Tech Stack**

### **Frontend**

* EJS (Embedded JavaScript)
* HTML5, CSS3
* Bootstrap / Custom CSS
* Server-side rendering (SSR)

### **Backend**

* Node.js
* Express.js
* REST APIs
* JWT Authentication
* Bcrypt.js for password hashing

### **Database**

* MongoDB
* Mongoose ORM

### **Cloud Storage**

* **Cloudinary** for property image uploads

---

## 🔐 **Authentication**

Wanderlust uses a secure authentication system:

* JWT tokens for session handling
* Passwords hashed with bcrypt.js
* Protected routes for property creation & management
* Logged-in user restrictions (only owner can edit/delete listing)

---

## 🏡 **Features**

### **User Features**

* Signup & Login with JWT auth
* View all holiday rental properties
* View property details including images, pricing, and location
* Fully responsive UI

### **Property Owner Features**

* Create a new listing
* Upload property images using Cloudinary
* Edit existing listings
* Delete listings
* Manage personal dashboard

### **Admin/Backend Features**

* MongoDB database integration
* Secure routes
* Error handling middleware
* Image upload with validations
* Mongoose schema & models

---

## 📸 **Image Handling with Cloudinary**

* Property images are uploaded directly to **Cloudinary servers**
* Secure storage with URL retrieval
* Fast image delivery and resizing
* Avoids local storage issues (scaling, hosting, etc.)

---

## 🗂️ **Project Structure**

```
Wanderlust/
│── models/
│   ├── user.js
│   ├── listing.js
│── routes/
│   ├── userRoutes.js
│   ├── listingRoutes.js
│── public/
│   ├── css/
│   ├── js/
│── views/
│   ├── index.ejs
│   ├── listings.ejs
│   ├── details.ejs
│   ├── login.ejs
│   ├── signup.ejs
│── middleware/
│── config/
│── app.js
│── package.json
```

---

## ⚙️ **Installation & Setup**

### **1️⃣ Clone the repository**

```bash
git clone https://github.com/ashish117840/Wanderlust
cd Wanderlust
```

### **2️⃣ Install dependencies**

```bash
npm install
```

### **3️⃣ Environment Variables**

Create a `.env` file:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

### **4️⃣ Run the server**

```bash
npm run dev
```

Server will run on:
`http://localhost:5000/`

---

## 📬 **API Endpoints**

### **Auth Routes**

| Method | Endpoint  | Description       |
| ------ | --------- | ----------------- |
| POST   | `/signup` | Register new user |
| POST   | `/login`  | Login and get JWT |

### **Listing Routes**

| Method | Endpoint            | Description                    |
| ------ | ------------------- | ------------------------------ |
| GET    | `/listings`         | Get all properties             |
| GET    | `/listing/:id`      | View property details          |
| POST   | `/listing/new`      | Create new listing (protected) |
| PUT    | `/listing/:id/edit` | Edit listing (protected)       |
| DELETE | `/listing/:id`      | Remove listing (protected)     |

---

## 🧪 **Security**

* Password hashing with **bcrypt.js**
* Token-based auth with **JWT**
* Middleware protection for CRUD operations
* Prevents unauthorized access to owner routes

---

## 📈 **Future Enhancements**

* Add user reviews & ratings
* Add booking system
* Add payment gateway (Razorpay)
* Add map/geo-location using Mapbox
* Add advanced property filters

---

## 👨‍💻 **Author**

**Ashish Kumar**
Full Stack Web Developer
GitHub: [https://github.com/ashish117840](https://github.com/ashish117840)
LinkedIn: [www.linkedin.com/in/ashish-kumar7000](http://www.linkedin.com/in/ashish-kumar7000)

---


