# Professional Intraday Trading App

A sophisticated trading application built for Whop with zone-based trading, multiple target levels, and professional UI.

## Features

- 🎯 **Zone-Based Trading**: Buy/Sell zones instead of single entry prices
- 📊 **Multiple Targets**: 8 target levels (4 upper, 4 lower)
- 📈 **Real-time P&L**: Live profit/loss tracking
- 📱 **Mobile Optimized**: Responsive design for trading on the go
- 🖼️ **Chart Screenshots**: Upload and view chart images
- 📋 **Trade Management**: Pending, Active, and Completed trade states
- 🎨 **Professional UI**: Dark theme with modern design

## Tech Stack

- **React 18** with Vite
- **Tailwind CSS** for styling
- **React Router** for navigation
- **Lucide React** for icons
- **Local Storage** for data persistence

## Getting Started

### Prerequisites

- Node.js 16+ 
- npm or yarn

### Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser

### Building for Production

```bash
npm run build
```

## Deployment to Vercel

### Option 1: Deploy via Vercel CLI

1. Install Vercel CLI:
   ```bash
   npm i -g vercel
   ```

2. Login to Vercel:
   ```bash
   vercel login
   ```

3. Deploy:
   ```bash
   vercel
   ```

### Option 2: Deploy via Vercel Dashboard

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Vercel will automatically detect the Vite framework
4. Deploy with default settings

### Vercel Configuration

The app includes a `vercel.json` configuration file that:
- Sets the build command to `npm run build`
- Configures the output directory as `dist`
- Sets up SPA routing with rewrites

## Project Structure

```
src/
├── components/
│   ├── ui/                 # Reusable UI components
│   ├── dashboard/          # Dashboard-specific components
│   └── trades/             # Trade-related components
├── pages/
│   ├── dashboard.jsx       # Main dashboard
│   ├── addtrade.js         # Add trade page
│   └── entities/
│       └── layout.jsx      # App layout with sidebar
├── entities/
│   └── Trade.js            # Trade data model
├── utils/
│   ├── index.js            # Utility functions
│   └── cn.js               # Class name utility
├── integrations/
│   └── Core.js             # File upload integration
└── data/
    └── sample-trades.js    # Sample data
```

## Usage

1. **Dashboard**: View all trades, statistics, and performance metrics
2. **Add Trade**: Create new trade setups with zones and targets
3. **Trade Management**: Update prices, activate trades, mark as complete
4. **Chart Analysis**: Upload and view chart screenshots

## Sample Data

The app includes sample trade data that loads automatically on first visit. You can clear localStorage to reset the data.

## Customization

- **Instruments**: Modify the symbol list in `entities/Trade.js`
- **Styling**: Update Tailwind classes or CSS variables
- **Features**: Add new components in the `components/` directory

## Support

For questions or issues, please check the code comments or create an issue in the repository.
