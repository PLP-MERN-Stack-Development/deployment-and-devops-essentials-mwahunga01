# MERN Full-Stack Application – Deployment & DevOps  
**Panaversity Learning Platform (PLP) – Cohort 2025**

A complete MERN stack blog application successfully deployed with **CI/CD pipelines**, **MongoDB Atlas**, and **production monitoring**.

## Live URLs
**Frontend (React + Vite):** https://plp-mern-blog-2025.vercel.app  
**Backend API (Node.js + Express):** https://mern-blog-backend-plp.onrender.com  
**API Health Check:** https://mern-blog-backend-plp.onrender.com/api/health

## Features Deployed
- Full CRUD Blog with Authentication
- Image Uploads
- JWT Authentication
- Responsive UI with Tailwind CSS
- MongoDB Atlas Production Database
- Automatic deployments on every push

## Deployment Platforms
| Part       | Platform     | URL                                   |
|------------|--------------|----------------------------------------|
| Frontend   | Vercel       | https://plp-mern-blog-2025.vercel.app  |
| Backend    | Render       | https://mern-blog-backend-plp.onrender.com |
| Database   | MongoDB Atlas| Cluster: `plp-cluster-2025`            |
| CI/CD      | GitHub Actions | Fully automated                     |

## CI/CD Pipelines (GitHub Actions)
All workflows pass on every push:
- `.github/workflows/frontend.yml` → Build & Deploy to Vercel
- `.github/workflows/backend.yml` → Test & Deploy to Render

## Environment Variables (Set in Render & Vercel)
**Backend (.env on Render)**
```env
MONGODB_URI=mongodb+srv://user:pass@plp-cluster-2025.mongodb.net/blogdb
JWT_SECRET=plp-super-secret-jwt-2025
NODE_ENV=production
PORT=10000
