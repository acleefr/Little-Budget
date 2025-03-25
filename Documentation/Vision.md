# Vision

## Context
Managing personal finances is hard without the right tools. I built a Notion database that tracks expenses, accounts, and cash flow. While it’s functional, it lacks automation, insights, and UX made for daily use—especially on mobile.

### Current Expense Entity
- **Date:** Date of the transaction
- **Amount:** Float
- **Status:** Text (ex: planned, paid)
- **Category:** Text (food, transport, etc.)
- **Rule:** Text (need, want, saving, income)
- **Bank Account:** Text (source or destination)

---

## Problems to Solve
The Notion setup has several limitations:
- Double entries required for internal transfers
- No automatic KPIs or analytics
- No "health score" overview
- No percentage breakdowns per category
- No saver profile or financial behavior insights
- No advice or recommendations
- Poor phone usability

---

## Product Vision
A personal finance **Web App (mobile-first)** that:
- Simplifies data entry
- Automatically calculates KPIs
- Gives insights & tips to improve saving behavior
- Shows real-time financial health
- Works well on phone screens
- Scalable to native iOS in the future

---

## Features

### 🎯 Main Pages
1. **Home**
   - Live financial health score
   - Real-time situation (available cash, upcoming expenses)
   - Distribution graphs
   - Key KPIs
2. **Expenses**
   - Full expense list (CRUD)
   - Simplified form for internal transfers
3. **Profile**
   - Wealth overview (assets, liabilities)
   - Saver profile based on behavior
4. **Situation**
   - Live vs End of Month projections
   - Comparison to last month
   - Category breakdown
   - Rules (Needs / Wants / Savings)
5. **Future Planning**
   - Simulations
   - Forecasts
   - Scenarios (buy a house, go on vacation, etc.)

---

### 📊 Data Structure (v2 Ready)
| Field          | Description                                        |
|--------------- |----------------------------------------------------|
| Date           | Date                                               |
| Status         | Planned / Sent / Paid                              |
| Category       | Food / Transport / Subscriptions / Housing etc.    |
| Type           | Income / Expense / Neutral                         |
| Rule           | Income / Need / Want / Saving / Doesn’t count      |
| Provenance     | Bank account or Sender                             |
| Destination    | Bank account or Beneficiary                        |
| Amount         | Float                                              |
| Notes          | Optional free text                                 |

### ✅ Technical Stack
- **Frontend:** ReactJS / NextJS (mobile-first)
- **Backend:** Python (FastAPI or Flask)
- **Database:** PostgreSQL
- **Hosting:** cPanel Server (V1)
- **Optional:** Chart.js or Recharts for graphs
- **V2:** iOS App Store version

---

### 🎯 Bonus Features (V2 / Future)
- AI-driven savings tips
- Auto-tagging expenses from CSV/Bank API
- Smart alerts (subscriptions growing, unusual spending)
- Export (PDF, CSV)
