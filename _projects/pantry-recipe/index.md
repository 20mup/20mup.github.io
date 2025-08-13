---
layout: project
title: "Pantry Recipes — Ingredient-Smart Finder"
date: 2025-08-13
description: "A café-styled recipe finder that matches your pantry, highlights missing ingredients, and builds a shopping list with one click."
tags: [React, UI/UX, CSS, Frontend, API]
role: "Design & Frontend Development"
tech:
  - React (Vite)
  - CSS (custom theme, dark mode)
  - TheMealDB API
  - canvas-confetti
links:
  demo: https://YOUR-DEMO-URL-HERE
  repo:  https://github.com/YOUR-USERNAME/pantry-recipes
cover_image: /assets/projects/pantry-recipes/cover.jpg
thumbnail:   /assets/projects/pantry-recipes/thumb.jpg
og_image:    /assets/projects/pantry-recipes/cover.jpg
---

> **TL;DR**: Search recipes by what you already have. The app compares your pantry terms against each recipe’s ingredients, shows how many you’d need to buy, and lets you add missing items to a shopping list (with confetti when you clear it 🎉). It’s wrapped in a warm café aesthetic with a dark/espresso mode.

## Why I built it
Cooking apps often assume you’ll shop for everything. I wanted something practical: type **what’s in your kitchen**, get **recipes with the fewest gaps**, and **one-tap add** missing ingredients to a **shopping list** you can actually use.

## Highlights
- **Ingredient matching** with fuzzy inclusion (e.g., “mozzarella” matches “mozzarella cheese”).
- **“Least to buy” ranking** so you cook with what you have.
- **Detail modal** with _You Have_ / _To Buy_ chips and steps.
- **Shopping list drawer** (copy/export, check off, clear + **confetti**).
- **Saved carousel** with mini cards & quick remove.
- **Polish**: image overlay, hover actions, line-clamped titles, chip wrapping, skeletons.
- **Dark/Espresso mode** toggle, persisted in localStorage.

## Screens
Place your screenshots in `/assets/projects/pantry-recipes/` and update file names below.

- **Grid View**  
  ![](/assets/projects/pantry-recipes/grid.jpg)

- **Detail Modal**  
  ![](/assets/projects/pantry-recipes/modal.jpg)

- **Shopping List Drawer**  
  ![](/assets/projects/pantry-recipes/drawer.jpg)

## Stack
- **Frontend**: React (Vite), custom CSS theme, responsive layout
- **API**: TheMealDB (open recipe dataset)
- **UX touches**: canvas-confetti, line clamps, hover overlays, dark mode

## How it works
1. **Search** — Enter comma-separated ingredients (e.g., `eggs, rice, chicken`).
2. **Match** — The app gathers candidate recipes and computes **missingCount**.
3. **Review** — Open any card to see the **You Have / To Buy** split.
4. **Shop** — Add all missing items to the **Shopping List Drawer**; copy the list or check items off as you go.

## Code snippets
```js
// Ranking by fewest missing ingredients (simplified)
detailed.sort((a, b) => a.missingCount - b.missingCount);
```

```css
/* Café theme tokens + dark mode */
:root{ --bg:#FAF7F2; --panel:#FFF8F0; --accent:#C1663D; }
:root[data-theme="dark"]{ --bg:#14110E; --panel:#1C1713; --accent:#D07A53; }
```

## Links
- **Live Demo**: [Open](https://YOUR-DEMO-URL-HERE)
- **Source**: [GitHub Repo](https://github.com/YOUR-USERNAME/pantry-recipes)

---

### Notes
- This project grew from UI cleanup (image scaling, chip wrapping) into a **portfolio-worthy** build with a cohesive visual language, accessibility touches, and persistent state.
- If you want to peek at the evolution, check the commit history: early image clamp → overlay and quick actions → modal → shopping drawer → dark mode → persistence & carousel polish.
