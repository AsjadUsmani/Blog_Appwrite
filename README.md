# 📝 Blog Web Application (React + Appwrite)

A full-stack blog web application built from scratch using **React**, **Redux Toolkit**, **React Router**, and **Appwrite**.  
This project focuses on real-world concepts like authentication, protected routes, file uploads, state management, and backend integration.

---

## 🚀 Features

### 🔐 Authentication
- User Signup & Login using Appwrite Auth
- Persistent login session
- Logout functionality
- Protected routes (only authenticated users can access certain pages)

### 📰 Blog Management
- Create new blog posts
- Edit existing posts
- Delete posts (author only)
- View all published posts
- View single post with rich text content

### 🖼️ Image Upload
- Upload featured images for blog posts
- Images stored in Appwrite Storage
- Image rendering using `getFileView()` (Free plan compatible)
- Safe handling of posts without images

### 🧠 State Management
- Global auth state using **Redux Toolkit**
- User session stored centrally
- Conditional UI rendering based on auth status

### 🛣️ Routing
- Client-side routing with **React Router v6**
- Dynamic routes for posts
- Route protection using custom `Protected` component
- Graceful handling of invalid routes

---

## 🛠️ Tech Stack

### Frontend
- React (Vite)
- Redux Toolkit
- React Router DOM
- React Hook Form
- Tailwind CSS

### Backend (BaaS)
- Appwrite
  - Authentication
  - Database
  - Storage

---


---

## ⚙️ Environment Variables

Create a `.env` file in the root and add:

```env
VITE_APPWRITE_URL=your_appwrite_endpoint
VITE_APPWRITE_PROJECT_ID=your_project_id
VITE_APPWRITE_DATABASE_ID=your_database_id
VITE_APPWRITE_COLLECTION_ID=your_collection_id
VITE_APPWRITE_BUCKET_ID=your_bucket_id
VITE_RTE_API_KEY=your_rte_api_key