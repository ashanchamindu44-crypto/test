# 🌤️ Weather Dashboard

![CI Pipeline](https://github.com/YOUR_USERNAME/weather-dashboard/workflows/CI%20Pipeline/badge.svg)
![Deploy](https://github.com/YOUR_USERNAME/weather-dashboard/workflows/Deploy%20to%20Production/badge.svg)

A modern, responsive weather dashboard application that displays current weather conditions and a 5-day forecast for any city worldwide.

## 👥 Group Information

| Role | Name | Student ID |
|------|------|------------|
| **DevOps Engineer & Full-Stack Developer** | K G ASHAN CHAMINDU | ITBNM-2313-0009 |

## 📖 Project Description

Weather Dashboard is a sleek, modern web application that allows users to:
- Search for weather information by city name
- View current weather conditions including temperature, humidity, wind speed, and visibility
- Check the 5-day weather forecast
- Quick-access popular cities with one click

The application features a beautiful glassmorphism design with smooth animations and is fully responsive across all device sizes.

## 🔗 Live Deployment

🌐 **Live URL:** [https://YOUR_USERNAME.github.io/weather-dashboard](https://YOUR_USERNAME.github.io/weather-dashboard)

> ⚠️ **Note:** Replace `YOUR_USERNAME` with your actual GitHub username after deployment.

## 🛠️ Technologies Used

- **Frontend:** HTML5, CSS3, JavaScript (ES6+)
- **Design:** Custom CSS with Glassmorphism effects
- **API:** OpenWeatherMap API
- **CI/CD:** GitHub Actions
- **Deployment:** GitHub Pages / Vercel / Netlify
- **Version Control:** Git & GitHub

## ✨ Features

- 🔍 **City Search:** Search weather for any city worldwide
- 🌡️ **Current Weather:** Real-time temperature, description, and conditions
- 📅 **5-Day Forecast:** Extended weather forecast with daily breakdowns
- 💨 **Weather Details:** Wind speed, humidity, feels-like temperature, visibility
- 🏙️ **Quick Cities:** One-click access to popular cities
- 📱 **Responsive Design:** Works perfectly on mobile, tablet, and desktop
- 🎨 **Modern UI:** Glassmorphism design with smooth animations
- 💾 **Local Storage:** Remembers your last searched city

## 🌿 Branch Strategy

We implemented the following branching strategy:

```
main          ← Production branch (protected, auto-deploys)
  │
  └── develop ← Integration branch
        │
        ├── feature/homepage-layout
        ├── feature/weather-api
        ├── feature/forecast-cards
        └── feature/responsive-design
```

- `main` - Production-ready code, protected branch
- `develop` - Integration branch for feature merging
- `feature/*` - Individual feature development branches

## 👤 Individual Contributions

### K G ASHAN CHAMINDU (ITBNM-2313-0009)
**Role:** DevOps Engineer & Full-Stack Developer

#### DevOps Contributions:
- ✅ Repository setup and configuration
- ✅ GitHub Actions CI/CD pipeline implementation (`ci.yml`, `deploy.yml`)
- ✅ Deployment setup and management
- ✅ Branch protection configuration
- ✅ Merge conflict resolution

#### Development Contributions:
- ✅ Complete Weather Dashboard UI (HTML/CSS)
- ✅ JavaScript application logic
- ✅ OpenWeatherMap API integration
- ✅ 5-day forecast feature
- ✅ Responsive design implementation
- ✅ Glassmorphism styling effects
- ✅ Local storage implementation

## 📦 Setup Instructions

### Prerequisites
- Node.js (version 18 or higher)
- Git
- OpenWeatherMap API key (free)

### Getting Your API Key
1. Go to [OpenWeatherMap](https://openweathermap.org/)
2. Sign up for a free account
3. Navigate to "API Keys" in your account
4. Copy your API key

### Installation

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/weather-dashboard.git

# Navigate to project directory
cd weather-dashboard

# Install dependencies
npm install

# Add your API key
# Open src/scripts/app.js and replace 'YOUR_API_KEY_HERE' with your actual API key

# Run development server
npm run dev
```

The application will open at `http://localhost:3000`

## 🚀 Deployment Process

### How the CI/CD Pipeline Works:

1. **CI Pipeline (ci.yml):**
   - Triggers on push to `main`, `develop`, and `feature/*` branches
   - Triggers on pull requests to `main` and `develop`
   - Checks out code, installs dependencies
   - Runs lint checks and builds
   - Verifies project structure

2. **Deployment Pipeline (deploy.yml):**
   - Triggers on push to `main` branch only
   - Builds the project
   - Deploys to GitHub Pages automatically

### Manual Deployment to Vercel:

1. Go to [vercel.com](https://vercel.com) and sign in with GitHub
2. Click "Add New Project"
3. Import your `weather-dashboard` repository
4. Set root directory to `src`
5. Click "Deploy"

## 📁 Project Structure

```
weather-dashboard/
├── .github/
│   └── workflows/
│       ├── ci.yml           # CI workflow
│       └── deploy.yml       # Deployment workflow
├── src/
│   ├── index.html          # Main HTML file
│   ├── styles/
│   │   └── style.css       # Stylesheet
│   └── scripts/
│       └── app.js          # JavaScript application
├── .gitignore              # Git ignore file
├── README.md               # This file
└── package.json            # Node.js configuration
```

## 🔄 Git Workflow Used

1. Created feature branches from `develop`
2. Made commits with conventional commit messages
3. Created pull requests with detailed descriptions
4. Merged approved PRs to `develop`
5. Merged `develop` to `main` for production releases

### Commit Message Convention:
- `feat:` - New feature
- `fix:` - Bug fix
- `docs:` - Documentation changes
- `style:` - Formatting changes
- `refactor:` - Code refactoring
- `test:` - Adding tests
- `chore:` - Maintenance tasks

## 🐛 Challenges Faced

1. **API Key Security:**
   - Challenge: Keeping API keys secure in public repository
   - Solution: Using environment variables and documenting the setup process

2. **Responsive Design:**
   - Challenge: Making glassmorphism effects work across all devices
   - Solution: Used CSS media queries and flexible grid layouts

3. **Merge Conflicts:**
   - Challenge: Resolving conflicts when merging feature branches
   - Solution: Used `git merge` with manual conflict resolution

## 📄 License

This project is created for educational purposes as part of the Advanced Git & DevOps Assignment.

---

**Module:** Systems Administration & Maintenance  
**Assignment:** Advanced Git & DevOps Team Collaboration  
**Instructor:** Isuru Samarappulige  
**Submission Date:** January 18th, 2025
