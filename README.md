# BUILD: BROKE BESTIE.EXE — PAYDAY SURVIVAL GAME

Create a fully functional, visually appealing, responsive web application called **Broke Bestie.exe**.

**Tagline:** "Survive payday, one questionable purchase at a time."

## PROJECT CONCEPT

Broke Bestie.exe is a gamified personal finance application designed to help people manage their money between paychecks.

The main problem is that many people struggle to understand whether their remaining money will cover upcoming bills, essential expenses, and daily purchases until their next payday.

Instead of being another traditional budgeting application, Broke Bestie.exe combines accurate financial tracking with retro gaming elements, funny messages, interactive purchase decisions, and visual warnings.

The app should feel like a nostalgic Y2K computer game combined with a clean, modern financial dashboard.

The app must support TWO selectable experiences:

1. **Bestie Mode:** A feminine, pink Y2K experience featuring Girl Math, playful dialogue, hearts, sparkles, and retro pop-ups.
2. **Classic Mode:** A gender-neutral retro gaming experience with arcade-inspired visuals, achievement badges, financial challenges, and more neutral language.

Both modes use the same financial data, features, and calculation logic.

Switching modes should instantly update the appearance and messaging without resetting the user's information.

---

## 1. WELCOME SCREEN AND MODE SELECTION

Design a memorable Y2K-inspired welcome screen.

Display:

BROKE BESTIE.EXE

"Survive payday, one questionable purchase at a time."

Include a large "START GAME" button.

After clicking Start Game, allow users to choose:

### BESTIE MODE 💗
"Budgeting, but make it cute."

Design:
- Baby pink (#F6D5E3)
- Berry pink (#A64D79)
- Cream (#FFF4E8)
- Lavender (#E8DDF5)
- Cherry red (#D94B65)

Visuals:
- Retro computer windows
- Pixel hearts
- Stars, bows, and sparkles
- Glossy pink buttons
- Cute Y2K icons
- Friendly and humorous messages

### CLASSIC MODE 🎮
"Beat the budget. Reach payday."

Design:
- Midnight navy (#18243A)
- Electric blue (#4A90E2)
- Mint green (#8DD9B5)
- Silver (#DDE4EC)
- Off-white (#F8FAFC)

Visuals:
- Retro arcade-inspired interface
- Pixel coins and progress bars
- Digital achievement badges
- Game-style notification windows
- Clean, readable buttons
- Straightforward but entertaining language

Allow users to change modes later from the dashboard.

Do not require users to identify their gender. These are optional appearance and personality preferences available to everyone.

---

## 2. FINANCIAL SETUP

After selecting a mode, guide users through a simple setup process.

Ask for:
- Current bank/card balance
- Physical cash balance
- Next payday date
- Expected paycheck amount (optional)
- Pay frequency (weekly, biweekly, twice monthly, monthly, or custom)
- Upcoming bills, amounts, and due dates
- Estimated essential expenses for the remaining pay period, including food, gas, and transportation

Keep the setup simple and visually appealing.

Include a "Try Demo Mode" button that loads fictional sample information for hackathon judges.

Store user data locally so it remains available after refreshing the page.

---

## 3. PAYDAY SURVIVAL DASHBOARD

Create an interactive dashboard displaying:

- Total available money
- Bank/card balance
- Physical cash balance
- Reserved money for bills and essentials
- Safe-to-spend balance
- Days remaining until payday
- Recommended daily spending allowance
- Payday countdown
- Wallet health bar
- Recent transactions
- Upcoming bills

Use a retro game-style dashboard layout.

### Wallet Health Bar

Display a prominent animated progress bar that represents the user's ability to financially survive until payday.

Use the following warning states:

GREEN: Financially on track based on the user's entered expenses.

YELLOW: Spending is approaching the available discretionary budget.

RED: Projected spending threatens bills or essential expenses.

Determine risk using actual financial calculations, not simply the percentage of the paycheck remaining.

When the user enters red status, display a dramatic retro warning window.

BESTIE MODE:

"🚨 GIRL, WE HAVE A PROBLEM! Your wallet is entering its broke era!"

CLASSIC MODE:

"🚨 LOW FUNDS ALERT! Your payday survival budget is at risk!"

Include:
- Rescue My Budget
- View Expenses
- Dismiss

Use warning animations without excessive flashing.

---

## 4. CASH AND CARD TRACKING

Create two separate wallet balances:

1. Bank/Card Wallet
2. Physical Cash Wallet

Users must be able to:
- Add income
- Withdraw cash
- Deposit cash
- Record card purchases
- Record cash purchases
- View transaction history

When a user withdraws $50:
- Bank balance decreases by $50
- Cash balance increases by $50
- Total money remains unchanged

Cash withdrawals are transfers, NOT expenses.

When users spend $20 cash:
- Cash balance decreases by $20
- Total available money decreases by $20

When users spend $20 using a card:
- Bank balance decreases by $20
- Total available money decreases by $20

Update the dashboard and wallet health bar immediately.

Validate transactions and prevent impossible transfers.

---

## 5. GIRL MATH VS. REAL MATH

This feature is available in Bestie Mode.

Create a fun interactive calculator called:

"GIRL MATH.EXE 💗"

Users can enter purchases and explore humorous financial scenarios.

### Scenario A: Cash Is Free

Girl Math:
"If I paid in cash, my card balance didn't change. So technically it was free!"

Real Math:
"Bestie, you still spent $25. Your total available money decreased."

### Scenario B: Shopping Sales

Girl Math:
"It was originally $100, but I paid $60. I basically made $40!"

Real Math:
"You spent $60. You paid $40 less than the original price."

### Scenario C: Returns

Girl Math:
"I returned a $50 dress. That's basically extra income!"

Real Math:
"You recovered $50 you previously spent. It isn't new income."

### Scenario D: Girl Dinner

Girl Math:
"I already have food at home, so dinner is free!"

Real Math:
"Using groceries you already purchased can help avoid spending more money tonight."

Show the humorous explanation first, followed by the accurate financial explanation.

Use cute pop-up windows, sparkles, and playful animations.

Girl Math must always be presented as a joke, never as an actual financial calculation.

### CLASSIC MODE ALTERNATIVE

Replace Girl Math with:

"MONEY MYTHS VS. MONEY FACTS"

Use the same underlying scenarios and accurate financial explanations, but with gender-neutral wording and retro arcade-style visuals.

Both versions should educate users about common spending misconceptions.

---

## 6. DELULU OR RESPONSIBLE? PURCHASE CHECKER

Create an interactive purchase simulator.

Users enter:
- Item name
- Purchase amount
- Payment method: Cash or Card

The app previews:
- Remaining total money
- Remaining bank or cash balance
- Updated safe-to-spend amount
- Updated daily spending allowance
- Effect on wallet health
- Risk of running short before payday

### BESTIE MODE RESULTS

GREEN:
"RESPONSIBLE BESTIE! 💚 You're staying on track!"

YELLOW:
"BESTIE, THINK AGAIN! 💛 This might make payday a little harder."

RED:
"DELULU ALERT! ❤️ Girl, your wallet cannot handle this right now!"

### CLASSIC MODE RESULTS

GREEN:
"PURCHASE CLEARED! You're within your spending plan."

YELLOW:
"CAUTION! This purchase reduces your financial flexibility."

RED:
"BUDGET OVERLOAD! This purchase could put essential expenses at risk."

Allow users to:
- Confirm Purchase
- Cancel
- Save for Later
- Try a Cheaper Price

Never subtract money until a purchase is explicitly confirmed.

If the user confirms a purchase, update the appropriate wallet and transaction history.

---

## 7. RESCUE MY BUDGET

Create an interactive rescue screen that activates when financial risk becomes high.

Display:
- Remaining total money
- Remaining days until payday
- Upcoming bills
- Essential expenses
- Estimated shortfall
- Available daily discretionary budget

Provide simple recommendations such as:
- Reduce nonessential spending
- Review upcoming subscriptions
- Use groceries already available
- Adjust optional purchases
- Prioritize bills and necessities

BESTIE MODE:

"Bestie, we're not panicking. We're making a comeback!"

CLASSIC MODE:

"Recovery Mode Activated. Let's rebuild your spending plan."

Do not suggest that users skip essential needs or required bills simply to improve their game score.

---

## 8. PAYDAY LEVELS AND ACHIEVEMENTS

Each pay period represents a game level.

Display:
- Current level
- Days completed
- Days remaining
- Payday progress bar
- Virtual achievement badges

Possible achievements:
- Payday Survivor
- Bill Boss
- Budget Bestie
- Savings Starter
- Money Master

Bestie Mode should use hearts, stars, and cute achievement cards.

Classic Mode should use arcade badges, trophies, and coins.

Use only virtual rewards, not real-money gambling or spending incentives.

Reward positive financial actions such as reviewing expenses, completing a budget, and preparing for bills.

Do not penalize users for low income or necessary purchases.

---

## 9. BESTIE ASSISTANT

Create a small retro-inspired assistant that appears through dialogue windows.

In Bestie Mode, use a cute pink character or pixel heart mascot.

Example messages:
- "New check, new chapter!"
- "Girl, the math isn't mathing!"
- "Bestie, rent is coming up!"
- "Your wallet needs a little TLC."
- "You made it to payday! Period!"

In Classic Mode, use a retro arcade assistant or simple robot icon.

Example messages:
- "New payday level unlocked."
- "Budget warning detected."
- "Upcoming payment approaching."
- "You're on track."
- "Level completed!"

Use rule-based messages for the initial prototype. Do not require an AI API to display basic financial feedback.

---

## 10. NAVIGATION AND SCREENS

Build these main screens:

1. Welcome / Mode Selection
2. Financial Setup
3. Payday Survival Dashboard
4. Wallet & Transactions
5. Purchase Checker
6. Girl Math / Money Myths
7. Rescue My Budget
8. Achievements

Use clear navigation with a sidebar on desktop and bottom navigation on mobile.

Provide a visible mode switcher in Settings or the dashboard header.

Keep the interface intuitive and avoid unnecessary complexity.

---

## 11. FINANCIAL CALCULATION RULES

All money must be stored and calculated using integer cents to avoid floating-point errors.

Total Funds = Bank Balance + Cash Balance

Reserved Funds = Unpaid Bills + Remaining Essential Expense Reserves

Safe-to-Spend = Total Funds − Reserved Funds

Daily Allowance = Maximum of zero and Safe-to-Spend divided by days remaining until payday.

Calculate wallet risk based on remaining funds, upcoming obligations, and planned spending.

Important:
- Do not count expected future paychecks as currently available money.
- Do not count cash withdrawals as spending.
- Do not count cash deposits as income.
- Do not double-count bills that have already been paid.
- Do not double-count purchases that are covered by an existing essential expense reserve.
- Allow users to update and correct transactions.
- Clearly distinguish available money from money reserved for bills.
- Show an accurate shortfall when reserved expenses exceed available funds.
- Handle payday dates, zero balances, and insufficient funds correctly.

The same calculations must apply in both modes.

---

## 12. TECHNICAL REQUIREMENTS

Use:
- React
- TypeScript
- Tailwind CSS
- Local storage for data persistence
- Reusable components
- Responsive layouts
- Lightweight animations

Do not require:
- User accounts
- Bank connections
- Payment processing
- Paid external APIs

Include a fully functional Demo Mode with realistic fictional data.

All buttons, forms, calculators, and navigation should work.

Avoid placeholder buttons and nonfunctional screens.

Make the app accessible, with readable text, clear financial labels, and color-independent warning indicators.

---

## 13. BUILD PRIORITIES

Prioritize functionality in this order:

1. Mode selection and theme switching
2. Financial setup and demo mode
3. Dashboard and wallet health bar
4. Cash and card transactions
5. Purchase checker
6. Girl Math / Money Myths
7. Budget rescue warnings
8. Achievements and animations

Build the core features before adding extra visual effects.

The final application should be polished enough for a live hackathon demonstration.

## FINAL PRODUCT GOAL

Broke Bestie.exe should help users understand whether their money can last until their next paycheck while making budgeting feel less intimidating.

It should combine financial education, practical money tracking, Y2K nostalgia, and lightweight gamification.

**The central idea: Budgeting shouldn't feel like punishment. It should feel like beating the level and making it to payday.**<div align="center">

<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />

  <h1>Built with AI Studio</h2>

  <p>The fastest path from prompt to production with Gemini.</p>

  <a href="https://aistudio.google.com/apps">Start building</a>

</div>
