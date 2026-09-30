# 🍎 Interactive Realistic Apple

An interactive HTML, CSS, and JavaScript project that creates a realistic-looking apple with smooth animations and interactive cutting effects.

The project demonstrates how SVG, CSS animations, and JavaScript event handling can be combined to create an interactive web experience without using external libraries.

---
## 🌐 Live Demo

🔗 [View Realistic Apple Live Demo](https://yuvashreedhanasekaren-coder.github.io/apple-project/)

## 🖼️ Project Preview

![Realistic Apple Preview](static/SVG_apple.png)
---

## 📌 Project Overview

This project starts with a realistic SVG-based apple displayed in the center of the page.

The apple supports multiple interactions:

- 🍎 Single click → Apple bounces
- 🔪 Double click → Knife animation starts
- 🍎 Apple is cut into 4 horizontal slices
- ✨ Each slice separates naturally after cutting
- 🌿 Stem and leaf remain attached to the apple
- 💨 Shadow reacts during the bounce
- 🔄 Refresh button resets the apple
- 📱 Simple and clean responsive webpage

The main goal of this project is to demonstrate interactive animations using only frontend technologies.

---

## ✨ Features

### 🍎 Realistic SVG Apple

The apple is created using SVG instead of using an external image.

It contains:

- Apple body
- Red gradient
- Highlight/shine
- Brown stem
- Green leaf
- Leaf veins

This makes the apple scalable without losing quality.

### 🖱️ Single Click Interaction

When the user clicks the apple once, the apple performs a smooth bounce animation.

### 🔪 Double Click Cutting

When the user double-clicks the apple:

1. Knife animation starts.
2. The knife performs three horizontal cuts.
3. The original apple is replaced by the cut version.
4. The apple separates into four horizontal slices.
5. Each slice moves slightly to create a natural cutting effect.

### 🔄 Refresh Apple

The refresh button restores the apple to its original state.

It resets:

- Original apple
- Apple position
- Bounce animation
- Cutting animation
- Knife
- Four slices
- Instructions

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| HTML5 | Page structure |
| CSS3 | Styling and animations |
| SVG | Apple, leaf, stem, knife and slices |
| JavaScript | User interactions and animation control |
| Git | Version control |
| GitHub | Source code hosting |
| GitHub Pages | Website deployment |

---

## 📂 Project Structure

```text
apple_project/
│
├── index.html
│
└── README.md
````

### `index.html`

Contains the complete project:

* HTML structure
* CSS styling
* SVG graphics
* CSS animations
* JavaScript interactions

### `README.md`

Contains the project documentation and usage information.

---

## 🎨 SVG Apple

The apple is created using SVG paths and gradients instead of an external image.

The SVG contains:

* Apple body
* Apple gradient
* Shine
* Stem
* Leaf
* Leaf veins

This allows the apple to remain sharp and scalable at different sizes.

---

## 🌈 Apple Gradient

A radial gradient is used to create the red apple appearance.

The gradient contains multiple shades ranging from light red to dark red to create depth and dimension.

---

## ✨ Apple Shine

A separate radial gradient creates the white reflection on the apple.

This gives the apple a more realistic glossy appearance.

---

## 🌿 Leaf

The leaf is created using an SVG path with a green linear gradient.

A separate SVG path is used for the leaf vein.

---

# 🎬 Animations

## 🍎 Bounce Animation

The single-click animation uses CSS `@keyframes`.

The apple moves:

```text
Normal
   ↓
Moves upward
   ↓
Moves slightly downward
   ↓
Small squash
   ↓
Returns to normal
```

The animation uses:

* `translateY`
* `scaleX`
* `scaleY`

to create a smooth bounce effect.

---

## 💨 Shadow Animation

The shadow changes its size and opacity during the bounce.

When the apple moves upward, the shadow becomes smaller.

When the apple returns downward, the shadow becomes larger.

This helps make the bounce look more natural.

---

# 🔪 Knife Animation

The knife is created using SVG.

It contains:

* Handle
* Grip
* Metallic blade
* Blade highlight
* Blade edge

The knife performs three horizontal cutting movements.

```text
Cut 1  ─────────────→

Cut 2  ─────────────→

Cut 3  ─────────────→
```

After the cutting animation, the apple changes into four horizontal slices.

---

# 🍎 Four Horizontal Slices

The cut apple consists of four separate sections:

1. Top slice
2. Second slice
3. Third slice
4. Bottom slice

SVG `clipPath` is used to define the shape of each slice.

Each slice has its own CSS animation so the pieces separate slightly after cutting.

---

# 🖱️ JavaScript Interaction

JavaScript controls the interaction and animation states.

The main elements are selected using:

```javascript
document.getElementById()
```

### Single Click

The apple listens for a click event and starts the bounce animation.

### Double Click

The apple listens for a double-click event and starts the cutting sequence.

The cutting sequence is:

```text
Double Click
     ↓
Hide instructions
     ↓
Knife animation
     ↓
Three cuts
     ↓
Original apple disappears
     ↓
Cut apple appears
     ↓
Four slices separate
```

### Refresh

The refresh button resets the entire animation state and displays the original apple again.

---

# 🧠 Single Click and Double Click Handling

Because a double-click contains click events, a short JavaScript delay is used for the single-click action.

The logic is:

```text
Single Click
     ↓
Short delay
     ↓
No second click?
     ↓
Bounce


Double Click
     ↓
Cancel pending click
     ↓
Start cutting
```

This prevents the apple from bouncing unnecessarily before the cutting animation starts.

---

# ▶️ How to Run Locally

No Python or server is required.

### Step 1

Clone the repository:

```bash
git clone https://github.com/yuvashreedhanasekaren-coder/apple-project.git
```

### Step 2

Open the project folder:

```bash
cd apple-project
```

### Step 3

Open `index.html` in a web browser.

---

# 🌐 GitHub Pages Deployment

This is a static HTML, CSS, JavaScript and SVG project, so it can be deployed using GitHub Pages.

### Deployment Flow

```text
Local Project
     ↓
Git
     ↓
GitHub Repository
     ↓
GitHub Pages
     ↓
Public Website
```

### GitHub Pages Setup

1. Open the GitHub repository.
2. Go to **Settings**.
3. Open **Pages**.
4. Select **Deploy from a branch**.
5. Select the `main` branch.
6. Select `/ (root)`.
7. Save the settings.

GitHub Pages will then publish the website.

---

# 📜 Git Workflow

The project uses Git for version control.

```bash
git status
```

```bash
git add .
```

```bash
git commit -m "Improve apple cutting animation"
```

```bash
git push origin main
```

---

# 📌 Project Checklist

* [x] HTML webpage
* [x] SVG apple
* [x] Apple gradient
* [x] Apple shine
* [x] Stem
* [x] Leaf
* [x] Leaf veins
* [x] Bounce animation
* [x] Shadow animation
* [x] Single-click interaction
* [x] Double-click interaction
* [x] SVG knife
* [x] Knife animation
* [x] Three horizontal cuts
* [x] Four apple slices
* [x] Slice separation animation
* [x] Refresh button
* [x] Reset functionality
* [x] GitHub repository
* [x] GitHub Pages deployment

---

# 🎯 Learning Objectives

This project helps demonstrate:

* HTML structure
* CSS styling
* CSS animations
* SVG graphics
* SVG gradients
* SVG clipping paths
* JavaScript DOM manipulation
* JavaScript event listeners
* Single-click and double-click handling
* Animation state management
* Git and GitHub
* GitHub Pages deployment

---

# 💡 What I Learned

This project demonstrates how HTML, CSS, SVG, and JavaScript can be combined to create an interactive visual experience without external animation libraries.

The project helped me understand:

```text
HTML
  +
CSS
  +
SVG
  +
JavaScript
  =
Interactive Web Experience
```

It also provided practical experience with animation control, DOM manipulation, SVG graphics, Git version control, and GitHub Pages deployment.

---

# 🔮 Future Improvements

Possible future improvements include:

* More realistic apple texture
* More detailed cutting animation
* Apple seeds and inner core
* Cutting sound effects
* Drag-to-cut interaction
* Mobile touch support
* More realistic physics
* Different fruits
* Multiple cutting directions
* Interactive fruit selection
* Dark mode
* Improved responsive design

---

## 📄 License

This project is created for learning, experimentation, and portfolio purposes.
