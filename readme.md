
# 🖼️ Image Transition Effect – Day 23 of 30 Days of JavaScript

A dynamic **before-and-after image comparison slider** built using **HTML**, **CSS**, and **JavaScript**. This project demonstrates how to visually compare two images (e.g., before & after editing) using a draggable vertical handle.

---

## ✨ Features

- ↔️ Interactive horizontal slider for comparing two images
- 📸 Smooth real-time image reveal on mouse movement
- ⚡ No external libraries required
- 🔧 Great for before/after showcases (e.g., background removal)

---

## 📸 Preview

Here’s what the Image Transition effect looks like:

![App Preview](https://raw.githubusercontent.com/Qasim-Rokeeb/Image-Transition/main/screenshot.png)

---

## 🌐 Live Demo

🔗 [View Live Project](https://qasim-rokeeb.github.io/Image-Transition)

---

## 🧱 Built With

- **HTML5** – Structure of the comparison slider
- **CSS3** – Styling, layout, and transition line
- **JavaScript** – Calculates mouse movement and updates image mask width

---

## 📁 Project Structure

```bash
Image-Transition-Effect/
├── index.html           # HTML layout with two overlapping images
├── style.css            # Slider and layout styles
├── script.js            # Core logic for slider movement
├── images/
│   ├── original.jpg     # Original image (full photo)
│   ├── transparent.png  # Edited image (e.g., background removed)
│   └── arrow.png        # Handle icon
├── screenshot.png       # Project preview image
└── README.md
```

---

## ⚙️ How It Works

1. The `.img-wrap` div holds the top image and changes width dynamically.
2. The mouse's X-position is tracked relative to the container.
3. The `mousemove` event sets:
   - `.img-wrap` width
   - vertical slider line position

```js
ImgBox.onmousemove = function(e){
  var boxWidth = (e.pageX - leftSpace) + "px";
  ImgWrap.style.width = boxWidth;
  line.style.left = boxWidth;
}
```

---

## 🧠 What I Learned

- How to create an image reveal effect with pure JavaScript
- How to use `offsetLeft` and `pageX` to calculate relative mouse movement
- How to overlay and mask images effectively using CSS

---

## 📅 Challenge

This is **Day 23** of my **30 Days of JavaScript** challenge.  
Follow me on X (Twitter) to keep up with the challenge:

📲 [@qasimrokeeb](https://x.com/qasimrokeeb)

---


## 🧩 Part of

**[30 Days of JavaScript Challenge](#)**
Follow the journey: [@qasimrokeeb](https://x.com/qasimrokeeb)
Hashtags: `#30DaysOfJS` `#JavaScript` `#FrontendDev` `Build In Public`

## 📜 License

This project is licensed under the [MIT License](LICENSE).
````

