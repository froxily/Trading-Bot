# Trading-Bot
Trading Simulator - A real-time stock market simulation app built with React that lets you practice trading with virtual money. Features 10 simulated stocks across different sectors, live price charts, buy/sell functionality.Perfect for learning trading strategies without financial risk. Built with React, Recharts, and Tailwind CSS.

# 📈 Trading Simulator

A real-time stock market simulation application that allows users to practice trading strategies with virtual money in a risk-free environment.

![Trading Simulator](https://img.shields.io/badge/React-18.x-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## 🌟 Features

- **Real-Time Price Updates** - Stock prices update every 2 seconds with realistic volatility
- **10 Diverse Stocks** - Trade across Technology, Finance, Energy, Healthcare, Retail, and more
- **Interactive Charts** - Visual price history with Recharts line charts
- **Buy/Sell Orders** - Execute instant market orders with live validation
- **Portfolio Management** - Track cash balance, holdings, and total portfolio value
- **Profit/Loss Tracking** - Real-time P&L calculations and percentage returns
- **Breaking News Events** - Random market-moving news that impacts stock prices
- **Order History** - Complete trade log with timestamps and details
- **Leaderboard System** - Compete with other traders for the highest portfolio value
- **Data Persistence** - Your portfolio and trades are saved automatically
- **Professional UI** - Dark-themed trading terminal aesthetic

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. **Clone or create the project**
```bash
npx create-react-app trading-simulator
cd trading-simulator
```

2. **Install dependencies**
```bash
npm install recharts lucide-react
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

3. **Configure Tailwind CSS**

Update `tailwind.config.js`:
```javascript
module.exports = {
  content: ["./src/**/*.{js,jsx,ts,tsx}"],
  theme: { extend: {} },
  plugins: [],
}
```

Update `src/index.css`:
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

4. **Copy the code**
- Replace `src/App.js` with the provided code
- Keep `src/index.js` as default

5. **Run the application**
```bash
npm start
```

The app will open at `http://localhost:3000`

## 🎮 How to Use

1. **Set Your Name** - Click "Set Name" in the top-right to join the leaderboard
2. **Select a Stock** - Choose from 10 available stocks in the left panel
3. **Monitor Prices** - Watch real-time price movements and chart updates
4. **Execute Trades**:
   - Enter the number of shares
   - Click BUY to purchase (if you have enough cash)
   - Click SELL to liquidate positions (if you own shares)
5. **Track Performance** - View your portfolio value, P&L, and return percentage
6. **Watch the News** - Breaking news events affect stock prices dynamically
7. **Compete** - Try to beat other traders on the leaderboard

## 📊 Stock Information

| Symbol | Company Name | Sector | Base Price | Volatility |
|--------|-------------|--------|------------|------------|
| TECH | TechCorp | Technology | $150 | Medium |
| FINX | FinanceX | Finance | $85 | Low |
| ENRG | EnergyPro | Energy | $120 | High |
| HLTH | HealthPlus | Healthcare | $200 | Medium |
| RTIL | RetailMax | Retail | $65 | Medium-High |
| AUTO | AutoDrive | Automotive | $95 | Medium |
| FOOD | FoodChain | Food | $45 | Low |
| AERO | AeroSpace | Aerospace | $180 | High |
| BANK | MegaBank | Banking | $110 | Medium |
| MINE | MineCorp | Mining | $75 | Very High |

## 🛠️ Built With

- **React** - Frontend framework
- **Recharts** - Chart visualization library
- **Lucide React** - Icon library
- **Tailwind CSS** - Utility-first CSS framework
- **LocalStorage API** - Data persistence

## 📁 Project Structure
```
trading-simulator/
├── public/
├── src/
│   ├── App.js          # Main application component
│   ├── index.js        # Entry point
│   ├── index.css       # Tailwind imports
│   └── ...
├── package.json
└── README.md
```

## 🎯 Game Rules

- **Starting Balance**: $50,000 virtual cash
- **Price Updates**: Every 2 seconds
- **News Impact**: Random events affect related stocks
- **Order Execution**: Instant market orders
- **Holdings**: Track multiple positions simultaneously
- **Data Persistence**: Saved in browser localStorage

## 🔧 Customization

### Adjust Starting Balance
```javascript
const INITIAL_BALANCE = 50000; // Change this value
```

### Modify Update Frequency
```javascript
setInterval(() => {
  // Price update logic
}, 2000); // Change interval (milliseconds)
```

### Add New Stocks
```javascript
const STOCKS = [
  // Add new stock objects here
  { symbol: 'NEW', name: 'NewCorp', sector: 'Tech', basePrice: 100, volatility: 0.03 }
];
```

## 🐛 Known Issues

- Leaderboard is stored locally (not synced across devices)
- Prices can theoretically go to zero (though unlikely with current volatility)
- No authentication system (single-user local storage)

## 🚀 Future Enhancements

- [ ] Limit orders and stop-loss functionality
- [ ] Options trading (calls/puts)
- [ ] Real market data integration
- [ ] Multi-user backend with database
- [ ] Historical performance analytics
- [ ] Technical indicators (RSI, MACD, Moving Averages)
- [ ] Mobile responsive improvements
- [ ] Dark/Light theme toggle
- [ ] Export portfolio reports

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 👨‍💻 Author

Built with ❤️ using Claude AI and React

## 🙏 Acknowledgments

- Recharts for beautiful chart components
- Lucide for clean iconography
- Tailwind CSS for rapid styling
- React community for excellent documentation

**Happy Trading! 📊💰**
