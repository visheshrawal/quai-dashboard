🌐 QUAI Network Dashboard
https://img.shields.io/badge/React-18.2.0-blue.svg
https://img.shields.io/badge/Vite-7.3.1-purple.svg
https://img.shields.io/badge/TailwindCSS-3.3.6-cyan.svg
https://img.shields.io/badge/License-MIT-green.svg

A real-time blockchain analytics dashboard for QUAI Network featuring interactive 3D visualizations, live data feeds, and comprehensive wallet analytics. Built for the Vibe Coding Hackathon.

https://via.placeholder.com/800x450/0f172a/ffffff?text=QUAI+Network+Dashboard

🚀 Live Demo
Demo Link • Video Walkthrough • GitHub Repository

✨ Features
🔍 Four Interactive Views
🌍 Network Pulse

Live 3D globe visualization with nodes lighting up for new blocks

Real-time block mining animation

Network health metrics and status indicators

Interactive globe controls (rotate, zoom, center)

📊 Dashboard

Real-time statistics cards (Wallet Balance, Total Blocks, Transactions)

Live block ticker with auto-refresh

Cache status indicators

Technical stack showcase

🔍 Wallet Profiler

Activity heatmap showing wallet usage patterns

Wallet DNA pie chart (Token Transfers, Contract Calls, Coin Transfers)

Advanced analytics on target wallet activity

Historical transaction analysis

📈 Token Flow

Interactive token transfer visualization

Network graph showing token movements

Volume and transfer statistics

Flow pattern analysis

⚡ Real-time Features
Live API data fetching from QUAI Scan

Auto-refresh every 10-15 seconds

Smart caching system for performance

Error handling with fallback data

WebSocket-like updates without page reload

🛠️ Tech Stack
Frontend
React 18 - UI Framework

Vite - Build tool & development server

Tailwind CSS - Utility-first CSS framework

React Globe GL - 3D globe visualization

ES6+ JavaScript - Modern JavaScript features

APIs & Services
QUAI Scan API - Blockchain data source

Supabase - Database & real-time logging

RESTful Architecture - Clean API integration

DevOps & Tools
Vercel - Deployment & hosting

Git - Version control

npm - Package management

ESLint - Code quality

PostCSS - CSS processing

📁 Project Structure
text
quai-dashboard/
├── src/
│   ├── App.jsx              # Main application component
│   ├── App.css              # Global styles
│   ├── main.jsx             # Application entry point
│   └── index.css            # Tailwind imports
├── public/                  # Static assets
├── index.html              # HTML template
├── package.json            # Dependencies & scripts
├── tailwind.config.js      # Tailwind configuration
├── postcss.config.js       # PostCSS configuration
├── vite.config.js          # Vite configuration
└── README.md               # This file
🚦 Getting Started
Prerequisites
Node.js 16+

npm or yarn

Modern web browser

Installation
Clone the repository

bash
git clone https://github.com/yourusername/quai-dashboard.git
cd quai-dashboard
Install dependencies

bash
npm install
# or
yarn install
Configure environment variables
Create a .env.local file:

env
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
Start development server

bash
npm run dev
# or
yarn dev
Open in browser
Navigate to http://localhost:5173

Build for Production
bash
npm run build
npm run preview
🔧 Configuration
API Endpoints
The dashboard uses these QUAI Scan APIs:

GET /api/v2/blocks - Latest blocks data

GET /api/v2/addresses/{hash} - Wallet information

GET /api/v2/stats - Network statistics

GET /api/v2/transactions/{hash}/logs - Transaction logs

Caching System
Blocks: 10-second cache duration

Wallet Data: 30-second cache duration

Transaction Logs: 15-second cache duration

Automatic refresh with cache fallback

Supabase Integration
Real-time event logging

User activity tracking

Analytics data storage

Secure API key management

🎨 Styling & Design
Color Scheme
Primary: #0f172a to #1e293b (gradient background)

Accent: #06b6d4 to #3b82f6 (cyan to blue gradients)

Success: #10b981 (green)

Warning: #f59e0b (amber)

Error: #ef4444 (red)

Typography
Font: System fonts with Tailwind's default stack

Headings: Bold with gradient text effects

Body: Clean, readable text with proper contrast

Responsive Design
Mobile-first approach

Breakpoints: sm:640px, md:768px, lg:1024px, xl:1280px

Flexible grid layouts with Tailwind's grid system

📊 API Integration Details
Data Flow
Client Request → React component triggers fetch

Cache Check → Check local cache before API call

API Call → Fetch from QUAI Scan endpoints

Data Processing → Format and transform API response

State Update → Update React state with new data

UI Render → Re-render components with fresh data

Supabase Log → Log event to database

Error Handling
Automatic retry on failed requests

Fallback to cached data when API fails

User-friendly error messages

Graceful degradation of features

🚀 Deployment
Vercel Deployment
Connect your GitHub repository to Vercel

Configure environment variables in Vercel dashboard

Deploy with automatic CI/CD

Set up custom domain (optional)

Environment Variables
Required for production:

env
VITE_SUPABASE_URL=https://your-project.supabase.co
VITE_SUPABASE_ANON_KEY=your-anon-key-here
VITE_QUAI_API_BASE=https://quaiscan.io/api/v2
📈 Performance Optimizations
Bundle Optimization
Code splitting with dynamic imports

Tree shaking to remove unused code

Minified production builds

Compressed assets

Runtime Optimizations
Efficient state management

Memoized components with React.memo

Debounced API calls

Lazy loading for heavy components

Network Optimizations
HTTP/2 support

Gzip compression

Browser caching headers

CDN for static assets

🧪 Testing
Manual Testing Checklist
All tabs load correctly

API data displays properly

Globe visualization works

Cache system functions

Responsive design on all devices

Error handling works

Supabase logging active

Browser Support
Chrome 90+

Firefox 88+

Safari 14+

Edge 90+

🤝 Contributing
Fork the repository

Create a feature branch

bash
git checkout -b feature/amazing-feature
Commit changes

bash
git commit -m 'Add amazing feature'
Push to branch

bash
git push origin feature/amazing-feature
Open a Pull Request

Development Guidelines
Follow existing code style

Write meaningful commit messages

Update documentation as needed

Add tests for new features

📚 Documentation
Component Documentation
Each component has inline comments

Prop types and default values documented

Usage examples in comments

API Documentation
QUAI Scan API Docs

Supabase Documentation

React Globe GL Docs

🐛 Troubleshooting
Common Issues
API Connection Failed

text
Solution: Check network connection and API endpoint availability
Globe Not Loading

text
Solution: Ensure Three.js dependencies are installed correctly
Build Errors

text
Solution: Clear node_modules and reinstall dependencies
Slow Performance

text
Solution: Enable caching, reduce API call frequency
Debug Mode
Enable debug logging in console:

javascript
localStorage.setItem('debug', 'true')
📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgments
QUAI Network for the blockchain infrastructure

QUAI Scan for providing the API

Vercel for hosting and deployment

Supabase for backend services

React Community for amazing tools and libraries

📧 Contact
Project Maintainer - Vishesh Rawal
Email - vishesh.rawal.dev@gmail.com
GitHub - @visheshrawal



<div align="center"> <p>Built with ❤️ for the QUAI community</p> <p>🚀 Happy coding!</p> </div>
🔗 Quick Links
Live Demo

Source Code

API Documentation

Issue Tracker

Changelog