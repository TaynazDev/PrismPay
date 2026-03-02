# Prism Pay

A beautiful, modern budget tracker with a dark glassmorphism aesthetic. Track transactions, set spending limits, analyze spending patterns, and split bills with friends—all in one sleek app.

🌐 **[Live Demo](https://taynazdev.github.io/PrismVault)**

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
- Invite friends by email — shared pots appear on their dashboard
- Real-time sync via Firebase Firestore
- Owner and member roles with shared deletion
- View each person's share amount at a glance

🎨 **Design & UX**
- Dark glassmorphism aesthetic with frosted glass cards
- Gradient accent color scheme (#f43f6e → #3b82f6)
- Staggered entrance animations on page load
- Smooth modal transitions with spring easing
- Hover states with soft gradient glows
- Fully responsive mobile design
- Smooth count-up animations for balance numbers

� **Authentication**
- Firebase Authentication (email & password)
- Sign up / sign in with user profile
- User name displayed in header with sign-out button
- All app content gated behind auth screen

💾 **Data Persistence**
- Transactions and budgets saved to scoped localStorage per user
- Group Pots stored in Firebase Firestore with real-time sync
- Data persists across sessions and devices (pots)

## Tech Stack

- **HTML5** — Semantic markup
- **CSS3** — Glassmorphism, animations, responsive grid
- **Vanilla JavaScript** — No frameworks
- **Firebase Auth** — Email/password authentication
- **Firebase Firestore** — Real-time shared Group Pots
- **Chart.js** — Interactive donut chart
- **Inter Font** — Clean sans-serif typography
- **localStorage API** — User-scoped client-side persistence

## Getting Started

1. Visit [taynazdev.github.io/PrismVault](https://taynazdev.github.io/PrismVault)
2. Sign up with your email and password
3. Start adding transactions
4. Set a budget to track spending
5. Create group pots and invite friends by email
6. All data is automatically saved

Or run locally:
```bash
# Clone the repository
git clone https://github.com/taynazdev/PrismVault.git

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
