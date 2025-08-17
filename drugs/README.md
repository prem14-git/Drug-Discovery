# Drugs Assistant - Full Stack Application

A comprehensive full-stack application for AI-powered drug discovery and pharmaceutical research, featuring molecular visualization, predictive analytics, and real-time collaboration tools.

![image](https://github.com/user-attachments/assets/b42cd80d-1e3c-4e5b-af05-930cde52adde)

https://drugs-assistant-345z.onrender.com (Live Link)

Use below login cerdentials [Since we have use Twilio Demo so otp will come to only registered phone number so use below credentials ]
- Email - test@gmail.com
- password - 1

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Configuration](#configuration)
- [Running the Application](#running-the-application)
- [Deployment](#deployment)
- [Environment Variables](#environment-variables)
- [API Endpoints](#api-endpoints)
- [License](#license)

## Features

### Backend
- Secure user authentication with JWT and bcrypt
- High-performance Redis caching layer
- MongoDB database with Mongoose ODM
- Multi-API integration:
  - Google Gemini for AI-driven drug analysis
  - MOLMIM for advanced molecular modeling
  - QWQ API for chemical property predictions
- Pharmaceutical news aggregation
- File upload handling with Multer
- Real-time collaboration with Socket.io
- PDF report generation

### Frontend
- Interactive molecular visualization (RDKit/NGL)
- Chemical structure editor (Ketcher)
- 3D molecular rendering (Three.js/Spline)
- Responsive Tailwind CSS UI
- State management with Zustand
- Animated transitions with Framer Motion
- Real-time updates via Socket.io
- AI-powered predictive analytics dashboard

## Technologies Used

### Problem Statement
The process of drug discovery is time-consuming, expensive, and often inefficient, with a high rate of failure in clinical trials. Traditional methods rely heavily on trial and error, requiring years of research and significant financial investment. Additionally, the complexity of biological systems and the vast chemical space make it challenging to identify promising drug candidates efficiently. 

Generative AI, with its ability to analyze large datasets, predict molecular interactions, and generate novel compounds, has the potential to revolutionize this process. However, there is a lack of accessible, user-friendly tools that leverage generative AI to assist researchers in accelerating drug discovery while reducing costs and improving success rates.

This application addresses these challenges by providing:

1. **AI-Augmented Discovery**: Integration with Google Gemini and specialized chemistry APIs to predict compound properties and generate novel structures
2. **Visualization Tools**: Interactive molecular viewers and editors to intuitively explore chemical space
3. **Collaboration Features**: Real-time sharing of research findings among team members
4. **Knowledge Integration**: Aggregation of relevant pharmaceutical news and research

### Backend Stack
- **Runtime**: Node.js (ES Modules)
- **Framework**: Express.js
- **Database**: MongoDB (Atlas)
- **Cache**: Redis (Upstash)
- **Authentication**: JWT + bcrypt
- **AI Services**: Google Generative AI, MOLMIM, QWQ
- **Real-time**: Socket.io
- **Utilities**: Axios, Multer, html2pdf

### Frontend Stack
- **Core**: React 18 + Vite
- **State**: Zustand
- **Styling**: Tailwind CSS + Animate
- **Cheminformatics**: RDKit, Ketcher, NGL
- **3D**: Three.js, Spline
- **UI**: Radix, Lucide, Heroicons
- **Charts**: To be implemented
- **Forms**: React Hook Form
- **Routing**: React Router

## Installation

### Prerequisites
- Node.js (v18+ recommended)
- MongoDB Atlas account
- Redis (Upstash recommended)
- Git

### Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/drugs-assistant.git
   cd drugs-assistant
  ```
PORT=5000
MONGODB_URI=mongodb+srv://<user>:<password>@cluster.mongodb.net/database
JWT_SECRET=complex_secret_here
GEMINI_API_KEY=your_google_ai_key
MOLMIM_API_KEY=your_molmim_key
QWQ_API_KEY=your_qwq_key
NEWS_API_KEY=your_newsapi_key
UPSTASH_REDIS_URL=redis://user:pass@host:port
ACCESS_TOKEN_KEY=access_secret
REFRESH_TOKEN_KEY=refresh_secret
```
##Running the Application
```
# Backend
npm run dev

# Frontend (in separate terminal)
cd frontend
npm run dev
```

