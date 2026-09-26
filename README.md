# SpendWise — Dashboard Shell 

A responsive dashboard shell for **SpendWise**, a personal budget and expense
tracker. This is the visual foundation of the capstone project: a clean,
modern dashboard layout built with CSS Grid and Flexbox, themed with CSS
custom properties, and responsive down to mobile.

No JavaScript, no interactivity — this week is about **layout and theme**.

## Files

- `index.html` — semantic dashboard structure
- `style.css` — layout, theme, responsive rules, micro-interactions
- `README.md` — this file

## What was built this week

### 1. Dashboard structure

Three regions, each styled as a distinct visual block:

- **Sidebar** — brand mark ("S"), app name "SpendWise", five nav links
  (Dashboard, Expenses, Categories, Reports, Settings), and a small footer.
- **Header / topbar** — page title, subtitle, a "this month" balance chip,
  and a user avatar.
- **Main content** — a 6-card grid of category tiles: Food, Transport, Rent,
  Entertainment, Savings, Utilities. Each card shows an icon, a trend chip,
  the category label, the amount, a meta line, and a progress bar.

Everything inside the cards is realistic static content — no calculations
yet.

### 2. CSS Grid + Flexbox

**CSS Grid** drives the page layout:

```css
.dashboard {
  display: grid;
  grid-template-columns: var(--sidebar-w) 1fr;
  min-height: 100vh;
}
