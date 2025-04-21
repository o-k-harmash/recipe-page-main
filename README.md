# Frontend Mentor - Recipe Page Main Solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/learning-paths/getting-started-on-frontend-mentor-XJhRWRREZd/steps/67f321e587e3060aad93b6bc/challenge/start).  
Frontend Mentor challenges help improve your frontend skills by building realistic projects.

---

## 📋 Table of Contents

- [Overview](#overview)
  - [Screenshots](#screenshots)
  - [Links](#links)
- [My Process](#my-process)
  - [Built With](#built-with)
  - [What I Learned](#what-i-learned)
  - [Continued Development](#continued-development)
  - [Useful Resources](#useful-resources)
- [Author](#author)

---

## 📌 Overview

### 📱 Screenshots

#### Mobile (iPhone SE – 375x667)

![Mobile Screenshot](<./screenshoots/_index.html(iPhone%2520SE)375x667.png>)

#### Responsive (1440x980)

![Responsive Screenshot](<./screenshoots/_index.html(Responsive)1440x980.png>)

The layout is fully responsive and adapts to various screen sizes while maintaining consistent proportions and paddings.

---

### 🔗 Links

- **Solution URL**: [View the solution on GitHub](https://github.com/o-k-harmash/recipe-page-main)
- **Live Site URL**: [View live demo](https://o-k-harmash.github.io/recipe-page-main/)

---

## 🔧 My Process

### ✅ Built With

- Semantic HTML5
- SEO with `<meta>` tags and other metadata
- CSS with cascade and inheritance
- CSS variables
- Relative data units
- Flexbox layout
- Minimal class usage — tag-based styling where appropriate

---

### 🧠 What I Learned

I deepened my understanding of:

### 🧠 What I Learned

While working with semantic `<table>` elements, I ran into one of those "designer vs HTML spec" situations.

#### 🍽️ Tables love structure — but they don’t like extra wrappers

- I was trying to **add spacing and alignment** inside `<td>`s by wrapping content in a `<div class="cell">`.
- Why? So I could control padding, margin, and font styling with modern CSS vars and utility styles.

#### ⚖️ But here’s the catch

- **`<td>` already acts like a box.**  
  It can take `padding`, `text-align`, `vertical-align`, etc. directly.
- By adding `<div>`s inside, I kinda **break the flow** of how tables are supposed to behave.
- Especially tricky when trying to align multiple rows consistently — browser rendering can get spicy.  
  (Some rows may look slightly off depending on the line-height, borders, or if the content inside wraps.)

#### ✅ Takeaway

If you’re building a **semantic data table**, try to:

- Style `<td>` directly where possible.
- Use `padding` and `text-align` instead of nesting `div`s.
- Only add `div` wrappers if you’re doing something extra custom — like grid/flex inside a cell, icons, or pseudo-elements.

Tables are like old souls. They just want to present data cleanly — don’t mess with their chi unless you have to.

- **Semantic HTML5**: Using meaningful tags and clean structure
- **Custom attributes**: Including `data-*` attributes when needed
- **CSS cascade and inheritance**: Applying styles thoughtfully using the cascade and specificity
- **Efficient selector usage**: Combining selectors and using combinators instead of over-classing
- **Text wrapping in flex children**: When using `white-space: nowrap` or similar styles inside an element that’s nested in a flex item, the flex child must have an explicit `min-width` (e.g. `min-width: 0`) to allow proper shrinkage. Without it, long inline content can break layout constraints and prevent truncation or wrapping from working as expected.
- **Font sizing issues in `inline-flex`**: Elements using `display: inline-flex` may not always respect inherited `font-size` and `line-height`, leading to inconsistent typography unless these values are explicitly defined.

I also focused on building a structure that’s both **logical** and **scalable**, avoiding unnecessary classes when tag-based styling suffices.

---

### 🚀 Continued Development

I plan to build on these core concepts and use them as a solid foundation for more advanced layouts and components. Future learning will expand into accessibility (a11y), reusable design systems, and responsiveness using modern CSS tools like `grid`, `clamp()`, and container queries.

---

### 📚 Useful Resources

- [HTML – web.dev](https://web.dev/learn/html) – A great deep-dive into modern semantic HTML.
- [CSS – web.dev](https://web.dev/learn/css) – Covers key CSS concepts like specificity, cascade, and layout techniques.
- [Git Fundamentals – Epic Web](https://www.epicweb.dev/tutorials/git-fundamentals) – A great beginner-friendly intro to Git and GitHub.

---

## 👤 Author

- Frontend Mentor – [@o-k-harmash](https://www.frontendmentor.io/profile/o-k-harmash)
- GitHub – [@o-k-harmash](https://github.com/o-k-harmash)
