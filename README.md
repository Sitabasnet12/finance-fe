# **Finance Tracker App**

## **1. Project Overview**
The **Finance Tracker App** is a web application designed to help users manage their finances by tracking income, expenses, and overall balance. The app offers users the ability to log in, record financial transactions, view their current balance, and analyze their spending habits through visual reports. The application will be developed using the MERN (MongoDB, Express.js, React.js, Node.js) stack, with the frontend and backend deployed separately.

---

## **2. Features**

### **User Authentication**
- Users can create an account and log in securely.
- User sessions will be managed to ensure data privacy.

### **Income and Expense Tracking**
- Users can add income and expenses with a description, date, and amount.
- Transactions will be stored and categorized for easy retrieval.

### **Balance Overview**
- The app will display the current balance based on the logged income and expenses.
- Users can see a breakdown of their financial status at a glance.

### **Financial Reports**
- **Pie charts**: Display the proportion of different categories of expenses.
- **Line graphs**: Show income and expense trends over time.

### **Pages**
1. **Registration Page**: User creation interface.
2. **Login Page**: User authentication interface.
3. **Dashboard**: Overview of current balance and quick add transaction feature.
4. **Transactions Page**: Detailed list of all transactions with options to add, edit, or delete.

---

## **3. Technology Stack**
- **Frontend**: React.js
- **State Management**: Context API
- **UI Library**: React-Bootstrap
- **Charts**: Chart.js or Recharts
- **Backend**: Node.js with Express.js
- **Database**: MongoDB (hosted on MongoDB Atlas)
- **Authentication**: JWT (JSON Web Tokens)

### **Deployment**
- **Frontend**: Deployed on Netlify or Vercel
- **Backend**: Deployed on Render or Cyclic

---

## **4. Database Design**

### **Users Collection**
| Field      | Type       | Description                     |
|------------|------------|---------------------------------|
| `_id`      | ObjectId   | Unique identifier              |
| `username` | String     | User's username                |
| `email`    | String     | User's email (unique)          |
| `password` | String     | Hashed password                |
| `createdAt`| Date       | Account creation timestamp     |

### **Transactions Collection**
| Field        | Type       | Description                                      |
|--------------|------------|--------------------------------------------------|
| `_id`        | ObjectId   | Unique identifier                                |
| `userId`     | ObjectId   | Reference to Users collection                    |
| `type`       | String     | Income or Expense                                |
| `amount`     | Number     | Transaction amount                               |
| `date`       | Date       | Transaction date                                 |
| `description`| String     | Details about the transaction                   |
| `createdAt`  | Date       | Transaction creation timestamp                  |

---

## **5. Security Considerations**
- Passwords will be hashed before storage using **bcrypt**.
- **JWT** will be used for authentication with secure cookie storage.
- **HTTPS** will be enforced on both frontend and backend deployments.

---

## **6. Project Plan**

### **Phase 1: Planning & Design (Day 1)**
- **Requirement Gathering**: Finalize app features and scope.
- **Wireframing & UI Design**: Create wireframes for each page.
- **Technology Setup**: Set up Git repository and CI/CD pipeline.

### **Phase 2: Backend Development (Day 2-3)**
- **User Authentication**: Develop the user login and registration API.
- **Transaction Management**: Create APIs for adding, editing, and deleting transactions.
- **Balance Calculation**: Implement logic for balance computation based on transactions.
- **Data Security**: Implement JWT authentication and secure storage practices.

### **Phase 3: Frontend Development (Day 3-5)**
- **Sign Up and Login Page**: Develop the user sign up and login interface.
- **Dashboard Page**: Implement the dashboard with balance overview and quick transaction add.
- **Transactions Page**: Develop the transaction list with edit and delete functionality.

### **Phase 4: Manual Testing (Day 5-6)**
- **E2E Testing**: Perform end-to-end testing to ensure app functionality.

### **Phase 5: Deployment (Day 7)**
- **Backend Deployment**: Deploy the backend to Heroku or AWS.
- **Frontend Deployment**: Deploy the frontend to Netlify or Vercel.
- **Final Testing**: Perform a full system test post-deployment.

### **Phase 6: Post-Launch (Day 8)**
- **Monitoring**: Set up monitoring and error tracking.
- **Feedback & Iteration**: Gather user feedback and iterate on the product.
- **Documentation**: Finalize project documentation and API references.

---

## **7. Contact**
For questions or contributions:
- Email: `your-email@example.com`
- GitHub: [your-username](https://github.com/your-username)
