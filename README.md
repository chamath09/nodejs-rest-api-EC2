# Node.js REST API with MongoDB and Automated Deployment on AWS EC2

![License](https://img.shields.io/badge/license-MIT-green)  
![Node.js](https://img.shields.io/badge/Node.js-v16.x-green)  
![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-brightgreen)  
![AWS EC2](https://img.shields.io/badge/AWS-EC2-orange)  
![GitHub Actions](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-blue)

## 🚀 Project Overview

This repository contains a **Node.js REST API** connected to **MongoDB** and deployed on an **AWS EC2** instance using **GitHub Actions** for continuous integration and delivery (CI/CD). The project is designed to automate the deployment process, ensuring a seamless and scalable infrastructure.

### 🌟 Key Features

- **Node.js REST API**: 
  - Implements CRUD operations for managing data.
  - Integrated with **MongoDB Atlas** for database management.
  
- **MongoDB Integration**: 
  - Secure connection to MongoDB Atlas for efficient data handling.
  - Environment variables for sensitive information.

- **GitHub Actions CI/CD**:
  - Automates testing, building, and deployment.
  - Deploys changes to **AWS EC2** on every push to the `main` branch.

- **AWS EC2 Hosting**:
  - Configured to run the Node.js application in a production environment.
  - Ensures scalability and high availability.

- **Security and Best Practices**:
  - Implements **Content Security Policy (CSP)**.
  - Uses **GitHub Secrets** for managing sensitive data.

---

## 🛠️ Technologies Used

- **Node.js**: Backend framework for building REST APIs.
- **MongoDB**: NoSQL database for managing dynamic data.
- **Express.js**: Lightweight web framework for Node.js.
- **GitHub Actions**: CI/CD for automated workflows.
- **AWS EC2**: Cloud hosting for the application.
- **MongoDB Atlas**: Managed database service.
- **Docker**: (Optional) Containerize the application for deployment.

---

## 🚀 Deployment Workflow

1. **Local Development**:
   - Develop and test the application locally.
   
2. **Push to GitHub**:
   - Code changes are pushed to the `main` branch.

3. **GitHub Actions Workflow**:
   - Runs tests and builds the application.
   - Deploys the application to **AWS EC2**.

4. **AWS EC2 Deployment**:
   - Pulls the latest changes and runs the application.
   - Connects to **MongoDB Atlas** for data storage.

---

## 📁 Project Structure

```
nodejs-rest-api-EC2/
├── src/
│   ├── models/         # Mongoose schemas
│   ├── routes/         # API route handlers
│   ├── controllers/    # Business logic for API
├── .github/workflows/  # GitHub Actions CI/CD workflow
├── .env                # Environment variables
├── app.js              # Main application file
├── README.md           # Project documentation
```

---

## 🔧 Getting Started

### Prerequisites

- **Node.js**: v16.x or higher
- **MongoDB Atlas** account
- **AWS EC2** instance with Node.js installed

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/chamath09/nodejs-rest-api-EC2.git
   cd nodejs-rest-api-EC2
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   - Create a `.env` file in the root directory:
     ```
     MONGO_URI=your_mongodb_connection_string
     PORT=5000
     ```

4. Start the server locally:
   ```bash
   npm start
   ```

---

## 🚀 Deployment to AWS EC2

1. **Set up AWS EC2**:
   - Launch an EC2 instance.
   - Install Node.js and MongoDB client.

2. **Configure GitHub Actions**:
   - Update the workflow file in `.github/workflows/deploy.yml`.
   - Add EC2 instance details and SSH credentials to GitHub Secrets.

3. **Trigger Deployment**:
   - Push changes to the `main` branch, and GitHub Actions will handle the deployment.

---

## 🛡️ Security

- Uses **GitHub Secrets** for secure management of sensitive data.
- Implements **CSP** and best practices to secure the API endpoints.

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repo, make changes, and submit a pull request.

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## ✨ Acknowledgments

- **GitHub Actions** for seamless CI/CD integration.
- **AWS** for reliable cloud infrastructure.
- **MongoDB** for robust database management.

