# BreakPoint Site — CSS System Starter  
GIT 414/515 — Lua Daniele

This repository contains my Practice: CSS System Starter assignment.  
I used the Home page from my surf capstone project to build a small, layered CSS architecture using the starter structure provided in class.


## 🎨 CSS Architecture
This project uses a six‑layer CSS system:

- reset  
- base  
- layout  
- components  
- utilities  
- overrides  

I added design tokens for color, typography, spacing, shape, and focus.  
All three project fonts are included: **Josefin Sans**, **Biryani**, and **Alegreya Sans SC**.

## Components
The Home page includes three repeated components styled in the `components` layer:

- navigation  
- surf spot cards  
- buttons  

## Utilities
I added three utilities 

- `.u-flex-center`  
- `.u-mb-2`  
- `.u-text-sm`  



## States & Accessibility
The project includes:

- visible focus styles  
- hover and active states  
- a current‑page indicator using `aria-current="page"`  

##  Print Styles
A simple print block hides the hero and navigation and ensures clean printed output.

##  AI Disclosure
AI assistance was used to help  confirm layer order, and generate boilerplate structure.  
All CSS was written and tested by me.



# Capstone Responsive Layout System

This project extends my Module 2 CSS architecture into a production‑ready responsive layout system. I kept the layered structure (`reset`, `base`, `layout`, `components`, `utilities`, `overrides`) and added intrinsic grid layouts, container queries, preference queries, and content‑driven breakpoints. The goal was to build a layout that adapts to real content instead of device labels and stays readable at all sizes.

---

## Layout Architecture

### Layered CSS
I continued using the Module 2 architecture:
- **reset** – normalize spacing and box‑sizing  
- **base** – typography, colors, tokens  
- **layout** – page‑level wrappers and spacing  
- **components** – hero, cards, buttons  
- **utilities** – small helpers  
- **overrides** – print styles  

This keeps the stylesheet organized and predictable.

### Logical Properties
All spacing uses logical properties like:
- `padding-block`
- `padding-inline`
- `margin-inline-start`
- `inline-size`

This makes the layout more flexible and future‑proof.

---

## Responsive Foundation

The layout is fully fluid. I avoided fixed widths and used:
- `max-width` constraints  
- percentage sizing  
- flexible grid columns  
- intrinsic sizing (`auto`, `minmax()`)  

The nav, hero, intro, card grid, and footer all adapt without device assumptions.

---

## Grid Layouts

### Card Grid
The card grid uses intrinsic sizing and content‑driven breakpoints:
- 1 column by default  
- 2 columns at ~600px  
- 3 columns at ~900px  

These breakpoints were chosen based on when the content actually needed more space.

### Card Internal Grid
Each card uses:
```css
grid-template-columns: 1fr auto;


AI Disclosure 

I used AI assistance to help refine parts of my CSS architecture, especially around container queries, intrinsic grid sizing, and organizing my documentation. AI also helped me debug my navigation  

I verified all layout behavior myself in Chrome and Firefox at narrow, medium, wide, and 200% zoom. I tested keyboard focus, reduced‑motion behavior, and fallback behavior without container queries. I adjusted spacing, breakpoints, and component behavior based on real browser testing. All final decisions, code changes, and testing were done by me. 



