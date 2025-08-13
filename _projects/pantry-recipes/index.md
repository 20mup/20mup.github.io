---
layout: post
title: Pantry Recipes — Smart Cooking with What You Have
description: A foodie-inspired web app that finds recipes from the ingredients you already have, highlights what's missing, and builds a shopping list — all in a cozy café aesthetic with dark/light mode.
skills:
  - React (Vite)
  - CSS (custom theme)
  - TheMealDB API
  - Local Storage
  - UI/UX Design
  - canvas-confetti
main-image: /images/pantry/pantry_banner.jpg
---

# 🥘 Pantry Recipes — Smart Cooking with What You Have

> Turn whatever’s in your pantry into dinner — no endless scrolling, no wasted groceries.

<img src="/assets/images/pantry/dark-mode-pantry.jpg" alt="Pantry Recipes – dark mode hero and results" width="860"/>

---

## 🚀 TL;DR
**Pantry Recipes** lets you type the ingredients you already have and instantly surfaces recipes you can make. It ranks by **fewest missing ingredients**, shows a **You have / To buy** split, and can **add missing items to a shopping list**. Polished visuals include hover overlays, a saved carousel, and a **dark/espresso mode**.

---

## 🧩 Problem / 💡 Solution

**Problem:** Finding “what to cook tonight” is slow, and most apps assume you’ll shop for everything.  
**Solution:** A practical, aesthetic tool that:
- Suggests meals **based on your pantry**
- Clearly shows **what’s missing** (and how many)
- Lets you **one-click add** missing items to a **shopping list**

<img src="/assets/images/pantry/light-mode-pantry.jpg" alt="Pantry Recipes – light mode hero and results" width="860"/>

---

## ✨ Key Features

- 🥗 **Ingredient-based search** (comma-separated, e.g., `eggs, rice, chicken`)
- 🧮 **“Least to buy” ranking** for real-life cooking decisions
- 🔎 **Detail modal** with _You have_ / _To buy_ chips and steps
- 🛒 **Shopping list drawer** with copy/clear and persistence
- 💾 **Saved recipes** carousel (localStorage)
- 🌓 **Dark/espresso mode** toggle, persisted
- 🎉 **Delight details**: hover elevation, image overlays, confetti on clear

<img src="/assets/images/pantry/detailed-pantry.jpg" alt="Recipe detail modal with ingredients and steps" width="860"/>

---

## 💻 Tech Stack & Tools

![React](https://img.shields.io/badge/React-18-blue?style=flat)
![Vite](https://img.shields.io/badge/Vite-bundler-purple?style=flat)
![TheMealDB](https://img.shields.io/badge/API-TheMealDB-orange?style=flat)
![CSS](https://img.shields.io/badge/CSS-Custom%20Theme-green?style=flat)
![JavaScript](https://img.shields.io/badge/JavaScript-ES2023-yellow?style=flat)

---

## 🎥 Demo
<!-- Replace with your video or live link include if you have one -->
<!-- {% include youtube-video.html id="YOUR_VIDEO_ID" autoplay="false" %} -->

---

## 🧠 How It Works

1. **Search** — Enter pantry items; the app fetches candidate recipes from **TheMealDB** and normalizes ingredients.  
2. **Rank** — Each recipe is scored by **missingCount** and sorted ascending (“least to buy”).  
3. **Review** — Open a recipe to see matched vs. missing ingredients and the cooking steps.  
4. **Shop** — Add missing items to the **Shopping List Drawer**; check off or copy as text; list persists across refreshes.  
5. **Save** — Keep favorites in a **Saved** carousel for quick access later.

<img src="/assets/images/pantry/saved-pantry.jpg" alt="Saved recipes carousel" width="860"/>
<img src="/assets/images/pantry/shopping-list-pantry.jpg" alt="Shopping list drawer with missing items" width="420"/>

---

## 📎 Code Snippet

```js
// Rank by fewest missing ingredients (simplified)
detailed.sort((a, b) => a.missingCount - b.missingCount);
```

```css
/* Café theme tokens + dark mode */
:root{ --bg:#FAF7F2; --panel:#FFF8F0; --accent:#C1663D; }
:root[data-theme="dark"]{ --bg:#14110E; --panel:#1C1713; --accent:#D07A53; }
```

---

## 📖 Links

- **Live Demo:** YOUR_DEMO_URL
- **Source:** https://github.com/YOUR-USERNAME/pantry-recipes

---

> _From “What’s for dinner?” to “Dinner’s ready!” — using what you already have._
