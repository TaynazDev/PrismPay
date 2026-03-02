# Changelog

All notable changes to Prism Vault will be documented in this file.

## [1.2.0] - 2026-03-02

### 🎯 Firestore Group Pots & Invite Friends

**Live at:** https://taynazdev.github.io/PrismVault

#### Added
- Group Pots now stored in Firebase Firestore under each user's UID
- "Invite Friends" email input on pot creation form
- Email resolution against Firestore `users` collection — matched accounts get shared access
- Real-time pot sync via Firestore `onSnapshot` listener
- Owner / member badges on each pot card
- Owner can delete pot for all members; members can leave individually
- Status messages for unresolved invite emails
- Pots listener cleanup on sign-out
- Guard against duplicate event listener binding on re-init

#### Changed
- Pots no longer use localStorage — fully backed by Firestore
- `savePot()` wrapped in try/catch/finally for error resilience
- Auth toggle refactored to avoid recursive `arguments.callee` handler bugs

---

## [1.1.0] - 2026-03-02

### 🔐 Firebase Authentication

**Live at:** https://taynazdev.github.io/PrismVault

#### Added
- Firebase Authentication with email/password sign-in and sign-up
- Auth screen with glassmorphism card, mode toggle, and error handling
- User profile display in header with name and sign-out button
- All dashboard content gated behind authentication
- User UID written to Firestore `users` collection on sign-in/sign-up
- localStorage data scoped per user UID

---

## [1.0.0] - 2026-03-02

### 🎉 Initial Release

**Live at:** https://taynazdev.github.io/PrismVault

#### Added

**Dashboard & Analytics**
- Real-time financial summary with three stat cards (Balance, Income, Expenses)
- Smooth count-up animations on stat values on page load
- Donut chart component for spending breakdown by category using Chart.js
- Gradient color palette throughout (#f43f6e → #3b82f6)

**Transaction Management**
- Add transactions with description, amount, type (income/expense), and category
- Quick-add modal via floating action button (FAB) in bottom-right
- Transaction history list sorted by most recent
- Filter transactions by type (All, Income, Expenses)
- Delete individual transactions
- All transactions persisted to localStorage

**Budget Tracking**
- Set weekly or monthly spending limits
- Gradient progress bar showing spending percentage
- Color-coded warnings (normal → orange at 80% → red when exceeded)
- Real-time budget recalculation
- Change budget at any time

**Group Pots / Bill Splitting**
- Create named shared expense pots
- Add multiple people to each pot
- Automatic equal share calculation
- View each person's share breakdown
- Save multiple pots
- Delete pots when settled

**Design & UX**
- Dark glassmorphism aesthetic (#0a0a0f background)
- Frosted glass cards with `backdrop-filter: blur()`
- All interactive elements with hover states and gradient glows
- Staggered entrance animations for cards (fade in + slide up)
- Smooth modal open/close transitions with spring easing
- Fully responsive layout (desktop → mobile)
- Clean Inter sans-serif font from Google Fonts

**Data Persistence**
- localStorage for all user data (transactions, budget, pots)
- Automatic save on every action
- Data survives page refresh and browser restart

#### Categories Included
- Food
- Transportation
- Entertainment
- Shopping
- Bills
- Healthcare
- Salary
- Freelance
- Investment
- Other

(Quick-add modal uses simplified categories: Food, Transport, Subscriptions, Going Out, Clothes, Random, Other)

---

## Future Roadmap

- [ ] Export data as CSV
- [ ] Monthly spending trends chart
- [ ] Recurring transaction templates
- [ ] Dark/Light theme toggle
- [ ] Multi-currency support
- [ ] Expense tags and notes
- [ ] Savings goals tracking
- [ ] Sync transactions to Firestore
- [ ] Mobile app (React Native)
