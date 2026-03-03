# SPLITSER – CSS Feature Documentation

This document describes the visual components of the Splitser Dashboard and the specific CSS properties utilized for each.

---

## 1. Sidebar & Navigation
* **Flexbox (`display: flex`):** Used to align the logo and navigation links in a vertical column layout.
* **Glassmorphism:** Achieved using `backdrop-filter: blur(10px)` and a semi-transparent `rgba` background to create a "frosted glass" effect.
* **Transitions:** Applied `transition: 0.3s` to navigation links to ensure smooth color changes during hover states.

## 2. Header & User Identity
* **Flexbox (`display: flex`):** Used with `justify-content: space-between` to separate the page title from the user actions (Add button and Profile).
* **Gradients:** The "Add Expense" button uses `linear-gradient` for a modern appearance.
* **Border Radius:** Used `border-radius: 50%` on the user avatar to create a circle for the user's initials "SB" (Sibora Boba).

## 3. Financial Summary Cards
* **CSS Grid:** The `stats-grid` uses `grid-template-columns: repeat(auto-fit, minmax(250px, 1fr))` for an automated, responsive layout.
* **Accent Borders:** Utilized `border-left` with specific colors to visually categorize different financial data points.
* **Hover Interactions:** Used `transform: translateY(-8px)` to make cards lift when hovered on.

## 4. Advanced CSS Features
For HW2, these advanced CSS specification were utilized for specific layout challenges:

* **`display: flow-root`:** Applied to the main card containers (Expenses and Group Dynamics). This creates a **New Block Formatting Context**, ensuring that internal margins and content stay contained without affecting the outside layout.
* **`display: table` & `display: table-row`:** Used in the Analytics section to align category data into columns and rows without using HTML table tags.
* **`display: list-item`:** Applied to the Group Activity items. This allows `div` elements to behave as semantic list-items, enabling the use of `list-style-type: square` directly in CSS.
* **`display: contents`:** Used for item wrappers. This acts as a "ghost" container, removing itself from the layout while keeping its children (icons and text) as direct participants in the parent alignment.

## 5. Global Styling & Layout
* **Radial Gradients:** The page background uses a `radial-gradient` to create a professional look.
* **Media Queries:** Responsive design is managed with  `@media` rules that collapse the sidebar and stack dashboard cards vertically on smaller screens.
* **Box Shadows:** Strategic use of `box-shadow` on buttons and cards creates a glow affect for a modern look.