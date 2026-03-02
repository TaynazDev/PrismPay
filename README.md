# Prism Pay

A beautiful, modern budget tracker with a dark glassmorphism aesthetic. Track transactions, set spending limits, analyze spending patterns, and split bills with friends—all in one sleek app.

🌐 **[Live Demo](https://taynazdev.github.io/PrismPay)**

## Features

✨ **Dashboard Overview**
- Real-time balance, income, and expense tracking with smooth count-up animations
- Spending breakdown donut chart with gradient color scheme
- Three glassmorphic stat cards showing financial snapshot

💰 **Transaction Management**
- Add income and expense transactions with categories
- Quick-add modal for rapid logging (bottom-right FAB)
- Filter transactions by type (All, Income, Expenses)
- Delete individual transactions
- Sorted by most recent first

📊 **Budget Tracking**
- Set weekly or monthly spending limits
- Progress bar that fills with gradient color (pink → blue)
- Automatic warnings at 80% capacity (orange) and when exceeded (red)
- Real-time budget status updates

🎯 **Group Pots / Bill Splitting**
- Create named shared pots for group expenses
- Add multiple people and automatically calculate equal shares
- View each person's share amount at a glance
- Save multiple pots simultaneously

🎨 **Design & UX**
- Dark glassmorphism aesthetic with frosted glass cards
- Gradient accent color scheme (#f43f6e → #3b82f6)
- Staggered entrance animations on page load
- Smooth modal transitions with spring easing
- Hover states with soft gradient glows
- Fully responsive mobile design
- Smooth count-up animations for balance numbers

💾 **Data Persistence**
- All data saved to browser localStorage
- Transactions, budgets, and pots persist across sessions
- No account needed

## Tech Stack

- **HTML5** — Semantic markup
- **CSS3** — Glassmorphism, animations, responsive grid
- **Vanilla JavaScript** — No dependencies (except Chart.js)
- **Chart.js** — Interactive donut chart
- **Inter Font** — Clean sans-serif typography
- **localStorage API** — Client-side data persistence

## Getting Started

1. Visit [taynazdev.github.io/PrismPay](https://taynazdev.github.io/PrismPay)
2. Start adding transactions
3. Set a budget to track spending
4. Create group pots to split bills
5. All data is automatically saved locally

Or run locally:
```bash
# Clone the repository
git clone https://github.com/taynazdev/PrismPay.git

# Open index.html in a browser
open index.html
```

## File Structure

```
PrismPay/
├── index.html          # Single-file app (HTML + CSS + JS)
├── README.md           # This file
└── CHANGELOG.md        # Version history
```

## Browser Compatibility

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## License

MIT License — Feel free to use and modify!
