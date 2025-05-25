 # 🍽️ MealDash – Full Stack Food Ordering Web App

MealDash is a complete full-stack food delivery web application that allows users to browse, add food to their cart, place orders, and pay online. Built using the MERN stack (MongoDB, Express, React, Node.js) and integrated with Stripe for secure payment processing, MealDash provides a seamless and responsive food ordering experience.  

<br/>

## 🚀 Features

### ✅ User-Facing Features

**• User Authentication**

Secure sign-up and login functionality using JWT authentication. Users can register, log in, and manage their session.

**• Dynamic Food Menu**

Users can browse through a list of available food items fetched dynamically from the backend.

**• Shopping Cart**

Add, update, or remove food items in the cart. Cart state is maintained across sessions.

**• Order Placement & Payment**

Users can place orders and pay securely via Stripe payment gateway.

**• Order Tracking**

After placing an order, users can track the current order status.

**• Light/Dark Mode Toggle**

Aesthetic and user-friendly UI with support for both light and dark themes.

<br/>

### 🛠️ Admin Panel

**• Admin Authentication**

  Admins can log in securely to manage the platform.

**• Manage Food Items**

Add, update, or delete food items displayed on the frontend.

**• Order Management**

View all incoming orders and update their delivery status (e.g., pending, in-progress, delivered).

 <br/>

## 🧰 Tech Stack

| Layer                | Technology                      |
| -------------------- | ------------------------------- |
| **Frontend**         | React.js, Tailwind CSS          |
| **Backend**          | Node.js, Express.js             |
| **Database**         | MongoDB                         |
| **Authentication**   | JWT (JSON Web Tokens)           |
| **Payments**         | Stripe Payment Gateway          |
| **State Management** | React Context API / useReducer  |
| **Styling**          | Tailwind CSS, Responsive Design |

<br/>
 
## 📁 Folder Structure

**/client               → Frontend React App**

  /components         → Reusable UI components
  
  /pages              → Route-based pages (Home, Cart, Orders, etc.)

**/server               → Backend Express server**
    
/routes             → API route handlers (auth, food, orders)
      
 /controllers        → Business logic
      
 /models             → Mongoose schemas

**/admin                → Admin panel frontend**


<br/>

## 🔐 Authentication Flow

1.) Users register and login using their email and password.

2.) A JWT token is generated on login and stored securely in localStorage or HTTP-only cookies.

3.) Protected routes are implemented to restrict access to authenticated users only.

<br/>

## 💳 Payment Integration with Stripe

• Stripe is used to securely handle online payments.

• Users are redirected to a Stripe checkout page with order summary.

• Upon successful payment, the order is saved in the database and order status is updated.

<br/>

## 📦 How to Run the Project Locally

1.) Clone the repository
```
git clone https://github.com/your-username/MealDash.git

cd MealDash
```

2.) Install dependencies

```
# For server
cd server
npm install

# For client
cd ../client
npm install

# For admin
cd ../admin
npm install
```

3.) Set up environment variables

Create a .env file in the /server folder with the following variables:
```
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_jwt_secret
STRIPE_SECRET_KEY=your_stripe_secret
```

4.) Backend Setup

To setup the backend, follow the instructions given in [Project Setup Guide.](https://github.com/moali007/MealDash/blob/master/How%20To%20Run%20Project.pdf)


5.) Start the development servers
```
# Start backend
cd server
npm run start

# Start frontend
cd ../client
npm run dev

# Start admin panel
cd ../admin
npm run dev
```

<br/>

## 📸 Screenshots

<br/>

**🏠 Home Page**     <br/>


![Home Page.](https://github.com/user-attachments/assets/9cda4d58-94c5-46e8-b470-9789cee49feb)


<br/>



![](https://github.com/user-attachments/assets/3aaaee2e-70c5-421e-84c9-af9793a9cc2a)


<br/>

**🛒 Cart Page**

![](https://github.com/user-attachments/assets/5cf8dc1d-d502-45a9-b791-0a245e11743d)

<br/>

**🚚 Place Order Page**

![](https://github.com/user-attachments/assets/2e098109-6d9c-4bcf-bc7f-7596fa1f139c)




## 🙌 Future Enhancements

• Add delivery partner dashboard

• Add email notifications

• Add ratings & reviews for food items

<br/>

## 📃 License
This project is open-source and available under the [MIT License](https://opensource.org/license/mit).
