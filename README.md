# Mini Bloomberg Terminal

A professional financial dashboard with real-time market data, featuring a Bloomberg-style dark theme with orange accents. Built with React, TypeScript, Tailwind CSS, and Express.

![Mini Bloomberg Terminal](https://img.shields.io/badge/Mini%20Bloomberg%20Terminal-v2.0-orange)
![React](https://img.shields.io/badge/React-19-blue)
![TypeScript](https://img.shields.io/badge/TypeScript-5.9-blue)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-3.4-38B2AC)

## Features

### 11 Bloomberg-Style Commands

| Command | Description | Data Source |
|---------|-------------|-------------|
| **WEI** | World Equity Indices (S&P 500, NASDAQ, DAX, NIKKEI, etc.) | Yahoo Finance API |
| **GP** | Global Asset Performance Heatmap | Yahoo Finance API |
| **TOP** | Market News & Sentiment | Yahoo Finance API |
| **ECO** | Economic Calendar | Static Data |
| **SECF** | Sector Performance with ETF tracking | Yahoo Finance API |
| **INDU** | Industry Analysis by sector | Derived from sectors |
| **RV** | Relative Valuation comparison | Yahoo Finance API |
| **DES** | Company Description & Profile | Yahoo Finance API |
| **HP** | Historical Price data with OHLC tables | Yahoo Finance API |
| **FA** | Financial Analysis with quarterly results | Yahoo Finance API |
| **CHART** | Interactive Technical Charts | Yahoo Finance API |

### Terminal Features

- **Dark theme** with signature Bloomberg orange accents
- **Live ticker tape** with scrolling market data
- **Command autocomplete** with TAB key
- **Keyboard shortcuts** for quick navigation
- **Sidebar** with quick command buttons
- **Responsive design** for different screen sizes
- **Real-time data** from Yahoo Finance API

## Screenshots

*Add screenshots here*

## Tech Stack

### Frontend
- React 19
- TypeScript 5.9
- Tailwind CSS 3.4
- Vite 7
- Recharts (for charts)
- Lucide React (for icons)

### Backend
- Express 5
- Node.js 20+
- yahoo-finance2 (for market data)
- CORS enabled

## Getting Started

### Prerequisites

- Node.js 20+ installed
- npm or yarn package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/mini-bloomberg-terminal.git
cd mini-bloomberg-terminal
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server (runs both frontend and backend):
```bash
npm start
```

Or run them separately:
```bash
# Terminal 1 - Backend API
npm run server

# Terminal 2 - Frontend
npm run dev
```

4. Open your browser and navigate to:
```
http://localhost:5173
```

The API server will be running on `http://localhost:3001`

## Available Scripts

| Script | Description |
|--------|-------------|
| `npm run dev` | Start Vite development server |
| `npm run server` | Start Express API server |
| `npm start` | Start both frontend and backend |
| `npm run build` | Build production bundle |
| `npm run preview` | Preview production build |
| `npm run lint` | Run ESLint |

## API Endpoints

| Endpoint | Description |
|----------|-------------|
| `GET /api/health` | Health check |
| `GET /api/wei` | World Equity Indices |
| `GET /api/gp` | Asset Performance |
| `GET /api/secf` | Sector Performance |
| `GET /api/quote/:ticker` | Company Quote |
| `GET /api/history/:ticker` | Historical Prices |
| `GET /api/chart/:ticker` | Chart Data |
| `POST /api/quotes` | Multiple Quotes |
| `GET /api/news/:ticker` | Market News |
| `GET /api/financials/:ticker` | Financial Statements |
