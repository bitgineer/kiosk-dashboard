# 📊 Real-Time Kiosk Monitoring Dashboard

[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![Socket.IO](https://img.shields.io/badge/Socket.io-010101?&style=for-the-badge&logo=Socket.io&logoColor=white)](https://socket.io/)
[![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)](https://sqlite.org/)
[![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)

> **An enterprise monitoring solution I designed to manage 500+ Bitcoin ATMs across the United States, achieving 95%+ uptime and reducing emergency response times by 70%.**

## ⭐ My Role: Architect & Project Lead

As the architect for this project, my role was to design a comprehensive, real-time monitoring solution to solve critical operational challenges. I was responsible for:
- **Designing the overall system architecture**, including the background monitoring engine, the real-time dashboard server, and the data persistence strategy.
- **Architecting the automated alert system** using the Telegram API to deliver critical issue notifications instantly.
- **Defining the requirements for the interactive frontend**, including the live maps, analytics charts, and issue tracking interface.
- **Directing the development process** using AI tools to rapidly build and deploy the solution.

The following document describes the technical details and features of the system that was built based on my architecture and direction.

## 🎯 System Overview

A comprehensive real-time monitoring system that provides 24/7 surveillance of Bitcoin ATM networks, automated issue detection, emergency response coordination, and detailed analytics for operations teams.

## 🚀 Key Achievements

- **🏆 95%+ uptime** across 500+ Bitcoin ATM network
- **⚡ 70% reduction** in emergency response time
- **🔄 Automated monitoring** running every 10 minutes
- **📱 Real-time alerts** via Telegram for critical issues
- **📈 Interactive dashboards** with maps, charts, and analytics

## 🏗️ Architecture Overview

```
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   Ops.js        │───▶│   API Monitor    │───▶│   Dashboard     │
│   Background    │    │   Status Check   │    │   Real-time UI  │
│   Workflow      │    │   Every 10min    │    │   Socket.IO     │
└─────────────────┘    └──────────────────┘    └─────────────────┘
         │                       │                       │
         ▼                       ▼                       ▼
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   SQLite        │    │   Telegram       │    │   Interactive   │
│   Historical    │    │   Notifications  │    │   Maps &        │
│   Analytics     │    │   Critical Alerts│    │   Charts        │
└─────────────────┘    └──────────────────┘    └─────────────────┘
```

## 🛠️ Technical Stack

### Backend Services
- **Node.js** - Server runtime and background processes
- **Express.js** - Web server and API endpoints
- **SQLite3** - Lightweight database for historical data
- **Node-cron** - Scheduled monitoring tasks

### Real-time Communication
- **Socket.IO** - Bidirectional real-time updates
- **Telegram Bot API** - Instant alert notifications
- **File Watching** - Monitor JSON status files for changes

### Frontend Dashboard
- **Vanilla JavaScript** - Lightweight client-side code
- **Chart.js** - Data visualization and analytics
- **Leaflet.js** - Interactive mapping
- **Bootstrap** - Responsive UI framework

### External Integrations
- **Custom APIs** - Proprietary ATM status endpoints
- **Local.lt** - Public tunneling for dashboard sharing
- **JSON File System** - Real-time status file monitoring

## 🔥 Core Components

### 🔄 **Ops.js - Background Workflow Engine**
```javascript
// Automated monitoring workflow
- API Status Polling (Every 10 minutes)
- Hardware Issue Detection
- Offline Kiosk Identification
- Critical Alert Triggering
- JSON Status File Updates
- Historical Data Logging
```

### 🖥️ **Dashboard.js - Express Server**
```javascript
// Real-time dashboard server
- REST API Endpoints
- Socket.IO Event Handling
- File System Watching
- Static Asset Serving
- Real-time Data Broadcasting
```

### 📊 **Frontend Dashboard Features**
- **Real-time Status Overview** - Live kiosk status grid
- **Interactive Maps** - Geographic distribution of issues
- **Analytics Charts** - Performance trends and metrics
- **Issue Tracker** - Historical problem resolution
- **Notification Center** - Alert management system

## 📋 Project Structure

```
kiosk-dashboard/
├── src/
│   ├── services/
│   │   ├── ops.js              # Background monitoring workflow
│   │   ├── dashboard.js        # Express server & Socket.IO
│   │   ├── apiService.js       # ATM API integration
│   │   ├── telegramService.js  # Notification service
│   │   └── databaseService.js  # SQLite operations
│   ├── routes/
│   │   ├── api.js              # REST API endpoints
│   │   ├── dashboard.js        # Dashboard routes
│   │   └── webhooks.js         # External webhook handlers
│   ├── models/
│   │   ├── Kiosk.js           # Kiosk data model
│   │   ├── Issue.js           # Issue tracking model
│   │   └── Analytics.js       # Analytics data model
│   └── utils/
│       ├── logger.js          # Winston logging
│       ├── validators.js      # Input validation
│       └── helpers.js         # Utility functions
├── public/
│   ├── css/
│   │   ├── dashboard.css      # Dashboard styles
│   │   └── responsive.css     # Mobile responsiveness
│   ├── js/
│   │   ├── dashboard.js       # Client-side dashboard
│   │   ├── charts.js          # Data visualization
│   │   ├── maps.js            # Interactive mapping
│   │   └── socketClient.js    # Socket.IO client
│   └── assets/
│       ├── icons/             # Status icons
│       └── images/            # UI images
├── views/
│   ├── dashboard.ejs          # Main dashboard view
│   ├── analytics.ejs          # Analytics page
│   ├── issues.ejs             # Issue tracker
│   └── partials/
│       ├── header.ejs
│       ├── sidebar.ejs
│       └── footer.ejs
├── data/
│   ├── offlineKiosks.json     # Real-time status file
│   ├── database.db            # SQLite database
│   └── logs/                  # Application logs
├── config/
│   ├── database.sql           # Database schema
│   ├── .env.example           # Environment template
│   └── config.js              # Application config
├── scripts/
│   ├── init.js                # Database initialization
│   ├── migrate.js             # Database migrations
│   └── deploy.js              # Deployment script
├── tests/
│   ├── unit/
│   ├── integration/
│   └── e2e/
├── docs/
│   ├── API.md                 # API documentation
│   ├── DEPLOYMENT.md          # Deployment guide
│   └── MONITORING.md          # Monitoring setup
├── package.json
├── docker-compose.yml
├── ecosystem.config.js        # PM2 configuration
└── README.md
```

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ and npm
- SQLite3
- Telegram Bot token
- ATM network API access

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourprofile/kiosk-dashboard.git
cd kiosk-dashboard
```

2. **Install dependencies**
```bash
npm install
```

3. **Configure environment**
```bash
cp config/.env.example .env
# Edit .env with your API keys and configuration
```

4. **Initialize database**
```bash
npm run db:init
```

5. **Start monitoring services**
```bash
# Start background monitoring
npm run ops:start

# Start dashboard server
npm run dashboard:start

# Or start both with PM2
npm run start:all
```

6. **Access dashboard**
```bash
# Local access
http://localhost:3000/dashboard

# Public tunnel (if configured)
https://your-tunnel.loca.lt/dashboard
```

## 📊 API Documentation

### Kiosk Status Endpoints
```javascript
GET    /api/kiosks                    // Get all kiosk statuses
GET    /api/kiosks/offline            // Get offline kiosks
GET    /api/kiosks/:id                // Get specific kiosk
PUT    /api/kiosks/:id/status         // Update kiosk status
```

### Analytics Endpoints
```javascript
GET    /api/analytics/uptime          // Get uptime statistics
GET    /api/analytics/issues          // Get issue trends
GET    /api/analytics/performance     // Get performance metrics
GET    /api/analytics/alerts          // Get alert history
```

### Real-time Events
```javascript
// Socket.IO Events
'kiosk_status_update'    // Real-time status changes
'new_issue_detected'     // New problem alerts
'issue_resolved'         // Problem resolution
'analytics_update'       // Updated metrics
```

## 🔧 Configuration

### Environment Variables
```env
# Database
DATABASE_PATH=./data/database.db
JSON_STATUS_FILE=./data/offlineKiosks.json

# ATM Network API
ATM_API_ENDPOINT=https://api.your-atm-network.com
ATM_API_KEY=your_api_key
ATM_API_TIMEOUT=30000

# Telegram Notifications
TELEGRAM_BOT_TOKEN=your_telegram_bot_token
TELEGRAM_CHAT_ID=your_chat_id

# Dashboard
DASHBOARD_PORT=3000
PUBLIC_TUNNEL_ENABLED=true
TUNNEL_SUBDOMAIN=atm-monitoring

# Monitoring
POLLING_INTERVAL=600000  # 10 minutes
ALERT_THRESHOLD=5        # Minutes offline before alert
CRITICAL_THRESHOLD=30    # Minutes for critical alert
```

### Monitoring Configuration
```javascript
// ops.js configuration
const monitoringConfig = {
  pollingInterval: 10 * 60 * 1000,  // 10 minutes
  retryAttempts: 3,
  timeoutDuration: 30000,
  alertThresholds: {
    warning: 5 * 60 * 1000,    // 5 minutes
    critical: 30 * 60 * 1000   // 30 minutes
  }
};
```

## 📈 Performance Metrics

- **Monitoring Frequency**: Every 10 minutes
- **Response Time**: < 5 seconds for status updates
- **Alert Latency**: < 1 minute for critical issues
- **Dashboard Load Time**: < 2 seconds initial load
- **Concurrent Users**: Supports 50+ simultaneous dashboard users

## 🔔 Alert System

### Alert Types
- **🟡 Warning**: Kiosk offline 5+ minutes
- **🟠 Critical**: Kiosk offline 30+ minutes  
- **🔴 Emergency**: Multiple kiosks in same region offline
- **🟢 Resolved**: Previously offline kiosk back online

### Notification Channels
- **Telegram**: Instant mobile notifications
- **Dashboard**: Real-time visual alerts
- **Email**: Daily/weekly summary reports
- **SMS**: Critical emergency alerts (if configured)

## 🛡️ Security & Reliability

### Security Features
- **API Authentication** - Secure endpoint access
- **Rate Limiting** - Prevent API abuse
- **Input Validation** - Sanitize all inputs
- **Error Handling** - Graceful failure management

### Reliability Features
- **Automatic Reconnection** - Handles API failures
- **Data Persistence** - SQLite for historical data
- **Process Monitoring** - PM2 for service management
- **Health Checks** - Self-monitoring capabilities

## 📊 Dashboard Features

### Real-time Status Grid
- Color-coded kiosk status indicators
- Last seen timestamps
- Issue duration tracking
- Geographic grouping

### Interactive Maps
- Kiosk location visualization
- Status-based map markers
- Zoom and filter capabilities
- Region-based analytics

### Analytics Charts
- Uptime trending over time
- Issue frequency analysis
- Response time metrics
- Performance comparisons

## 🧪 Testing

```bash
npm test                 # Run all tests
npm run test:unit        # Unit tests
npm run test:integration # Integration tests
npm run test:e2e         # End-to-end tests
npm run test:performance # Performance testing
```

## 📦 Deployment

### Production Deployment
```bash
# Using PM2
npm run deploy

# Using Docker
docker-compose up -d

# Manual deployment
npm run build
npm run start:production
```

### Monitoring Setup
```bash
# Start background monitoring
pm2 start ecosystem.config.js --only ops

# Start dashboard server
pm2 start ecosystem.config.js --only dashboard

# Monitor processes
pm2 monit
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/monitoring-enhancement`)
3. Commit your changes (`git commit -m 'Add monitoring enhancement'`)
4. Push to the branch (`git push origin feature/monitoring-enhancement`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙋‍♂️ Contact

**Tommy H** - Automation Engineer  
📧 Tommy.heredia24@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/theredia24)  

---

> **Technical Note**: This monitoring system demonstrates enterprise-grade real-time application development, API integration, and automated workflow management built with modern JavaScript technologies and AI-assisted development practices.
