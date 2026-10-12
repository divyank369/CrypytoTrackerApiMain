# Crypto Tracker

A React application for browsing cryptocurrency market data and individual coin details. It retrieves public market information from the CoinGecko API and displays historical prices in charts.

## Features

- Paginated cryptocurrency market list
- Currency selection for market values
- Coin details and historical price charts
- Client-side routing between the market and coin detail pages
- Loading and error states for API requests

## Technology

- React 18 and Vite
- React Router
- React Query
- Axios
- Chart.js and `react-chartjs-2`
- CoinGecko public API

## Requirements

- Node.js and npm
- Internet access to reach the CoinGecko API

## Run Locally

```bash
npm install
npm run dev
```

Open the local URL printed by Vite. The app uses the public CoinGecko API endpoint configured in `src/helpers/constants.js`; API availability and request limits are controlled by CoinGecko.

## Available Scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the Vite development server |
| `npm run build` | Create a production build in `dist/` |
| `npm run preview` | Preview the production build locally |
| `npm run lint` | Run ESLint |

## Project Structure

```text
src/
├── component/   # Shared UI and coin chart components
├── context/     # Currency state
├── helpers/     # API client and shared constants
├── pages/       # Market and coin detail pages
├── services/    # CoinGecko requests
└── App.jsx      # Application entry and routes
```
