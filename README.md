# Cryptocurrency Tracker

A React dashboard for exploring cryptocurrency market data and coin price history. The app loads market information from CoinGecko, shows a coin table, and provides a dedicated detail page with charts.

## Features

- Cryptocurrency market data with currency selection
- Coin detail pages with historical price visualizations
- Lazy-loaded page routes with a loading state
- React Query and Axios for data fetching
- Zustand for shared state
- Error boundary for rendering failures

## Built With

- React 18
- Vite
- React Router
- Axios and React Query
- Chart.js with `react-chartjs-2`
- Tailwind CSS and DaisyUI
- CoinGecko API

## Run Locally

Use a current Node.js installation and npm:

```bash
git clone https://github.com/divyank369/CrypytoTrackerApiMain.git
cd CrypytoTrackerApiMain
npm install
npm run dev
```

Vite prints the local development URL in the terminal. To create and preview a production build:

```bash
npm run build
npm run preview
```

## Repository Layout

```text
.
├── src/
│   ├── component/   # Navigation, coin table, loaders, and routing
│   ├── context/     # Currency context
│   ├── pages/       # Market home and coin detail views
│   ├── services/    # CoinGecko data requests
│   └── helpers/     # API client and shared constants
├── index.html
└── vite.config.js
```

Market data is requested from CoinGecko at runtime. Internet access and the provider's rate limits can affect requests.
