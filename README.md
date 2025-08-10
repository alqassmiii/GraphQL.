# GraphQL Profile Dashboard

A modern React.js dashboard application for visualizing user profile data from a GraphQL API. This application provides comprehensive insights into user progress, experience points, project completion, audit performance, and skill development.

## Features

### 📊 Data Visualization
- **Pure SVG Charts**: Custom-built SVG charts with no external charting dependencies
- **Interactive Elements**: Hover effects, tooltips, and responsive design
- **Dark/Light Theme Support**: Seamless theme switching with custom ThemeContext
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices

### 📈 Dashboard Components
- **XP Progression Chart**: Visualizes experience point accumulation over time
- **Level Progress Chart**: Shows current level progress with XP requirements
- **Skills Chart**: Displays technical skills proficiency levels
- **Technologies Chart**: Tracks technology usage and expertise
- **Success Rate Chart**: Project completion and audit performance metrics
- **Audit Performance Chart**: Detailed audit statistics and ratios

### 🎯 Key Metrics
- **Standardized XP Calculation**: Combined exercise and project XP (÷ 2048, displayed in KB)
- **Level Calculation**: Single source of truth using Math.max pattern
- **Project Statistics**: Completion rates, success/failure tracking
- **Audit Ratios**: Performance metrics and peer review statistics
- **Recent Activity**: Latest project progress and XP gains

### 🔧 Technical Features
- **GraphQL Integration**: Apollo Client for efficient data fetching
- **Custom Hooks**: Centralized data management with useUserData
- **CSV Export**: Download chart data for external analysis
- **Accessibility**: ARIA labels and screen reader support
- **Performance Optimized**: Memoized calculations and efficient rendering

## Technology Stack

- **Frontend**: React.js with functional components and hooks
- **Styling**: Tailwind CSS for responsive design
- **Data Fetching**: Apollo Client for GraphQL queries
- **Routing**: React Router for client-side navigation
- **Animations**: Framer Motion for smooth transitions
- **Deployment**: Vercel with SPA configuration

## Project Structure

```
src/
├── components/
│   ├── charts/                 # SVG chart components
│   │   ├── ModernXPProgressionChart.jsx
│   │   ├── ModernLevelProgressChart.jsx
│   │   ├── ModernSkillsChart.jsx
│   │   ├── ModernTechnicalSkillsChart.jsx
│   │   ├── ModernTechnologiesChart.jsx
│   │   ├── ModernSuccessChart.jsx
│   │   └── ModernAuditPerformanceChart.jsx
│   ├── profile/               # Profile-related components
│   │   ├── StatsCards.jsx
│   │   └── ProfileDashboard.jsx
│   └── ui/                    # Reusable UI components
├── hooks/
│   └── useUserData.js         # Custom hook for data management
├── services/
│   └── queries.js             # GraphQL query definitions
├── contexts/
│   └── ThemeContext.js        # Theme management
└── pages/
    └── Dashboard.jsx          # Main dashboard page
```

## GraphQL Queries

### Core Data Queries
- `GET_USER_BASIC_INFO`: User profile information
- `GET_USER_AUDIT_DATA`: Audit statistics and history
- `GET_USER_XP_AND_LEVEL`: Experience points and level data
- `GET_USER_SKILLS_DATA`: Technical skills proficiency
- `GET_USER_PROGRESS`: Project progress tracking
- `GET_USER_LEVEL_ONLY`: Standardized level calculation
- `GET_USER_TOTAL_XP`: Combined exercise and project XP

## Deployment

The application is configured for Vercel deployment with proper SPA routing support via `vercel.json`:
You can access the project by: https://graphql-e8mf.vercel.app/dashboard

### Login:
<img width="1502" height="794" alt="Screenshot 2025-08-10 at 6 29 09 PM" src="https://github.com/user-attachments/assets/155e9a01-1a88-4c6e-b35e-b7b846458b6a" />
<img width="1498" height="787" alt="Screenshot 2025-08-10 at 6 29 18 PM" src="https://github.com/user-attachments/assets/19feb55e-b796-4b02-8c3a-a8ec8202390e" />




### Dashboard :

<img width="2992" height="1436" alt="image" src="https://github.com/user-attachments/assets/4d4eca51-ef13-41be-95fd-9c819f49f914" />

<img width="2972" height="1378" alt="image" src="https://github.com/user-attachments/assets/2c1c8895-fcc0-4d6c-9fc7-6742e58944df" />

<img width="2954" height="1512" alt="image" src="https://github.com/user-attachments/assets/df283dc0-44dd-40a7-a77e-52c848ca0614" />










## Chart Components

### XP Progression Chart
- Displays cumulative XP growth over time
- Smooth bezier curves for visual appeal
- Interactive tooltips with project details
- Recent gains calculation (last 7 transactions)

### Level Progress Chart
- Donut chart showing current level progress
- XP requirements for next level
- KB format display for user-friendly values
- Progress percentage calculation

### Skills & Technologies Charts
- Bar charts for skill proficiency levels
- Technology usage tracking
- Interactive hover effects
- Responsive scaling

### Success & Audit Charts
- Project completion statistics
- Audit performance ratios
- Pass/fail rate visualization
- Performance trend analysis

## Data Flow

1. **GraphQL Queries**: Multiple specialized queries fetch different data aspects
2. **useUserData Hook**: Centralizes data processing and state management
3. **Data Processing**: Standardizes calculations and formats data for charts
4. **Component Rendering**: Charts receive processed data and render SVG visualizations
5. **User Interaction**: Hover effects, tooltips, and theme switching


## Browser Support

- Modern browsers with ES6+ support
- SVG rendering capabilities
- CSS Grid and Flexbox support
- GraphQL/Apollo Client compatibility

## 🛡️ Access Note

> 🚫 The source code for this project is private to protect intellectual property.  
> ✅ A live demo or code preview is available upon request for academic or professional purposes.

---

## 👨‍💻 Author

**Qassim Aljaafar**  
[LinkedIn](https://www.linkedin.com/in/qassim-aljaffer)  
📧 qassimhassan9@gmail.com  
📍 Manama, Bahrain

