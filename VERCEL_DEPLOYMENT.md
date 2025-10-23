# Frontend-Only Deployment

This is the **frontend-only** version of the Credit Card Statement Parser, optimized for Vercel deployment.

## ⚠️ Important: Backend Required

**This frontend requires a backend API server to function properly.**

The frontend is trying to connect to: `http://localhost:8000` by default, which only works when running locally.

### 🔧 To Make This Work on Vercel:

You need to deploy the backend separately and configure the frontend to use it.

#### Option 1: Deploy Backend on Railway (Recommended)
1. Go to [Railway.app](https://railway.app)
2. Create a new project
3. Connect your GitHub repository
4. Select the `backend` folder
5. Deploy the FastAPI backend
6. Copy the backend URL (e.g., `https://your-app.railway.app`)

#### Option 2: Configure Vercel Environment Variable
1. Go to your Vercel project settings
2. Navigate to "Environment Variables"
3. Add: `VITE_API_URL` = `https://your-backend-url.com`
4. Redeploy your frontend

### 📊 Current Deployment Status
- ✅ **Frontend**: Deployed on Vercel (this branch)
- ❌ **Backend**: Not deployed (needs separate deployment)

### 🚀 Quick Fix for Demo
To make the frontend work on Vercel temporarily, you can:
1. Deploy the backend on Railway, Render, or Heroku
2. Set the `VITE_API_URL` environment variable in Vercel
3. Redeploy the frontend

### 📝 Full Stack Deployment
For production deployment, consider deploying both:
- **Frontend**: Vercel (this branch)
- **Backend**: Railway, Render, or Heroku

See the main README.md for full deployment instructions.
