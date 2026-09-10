markdown
# Shivam Deb Barman — 3D Developer Studio & Portfolio

[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen?style=flat-square)](https://debbarmanshivam20-hue.github.io/Shivam3D_lab.com/)
[![Built With](https://img.shields.io/badge/Three.js-r128-black?style=flat-square&logo=three.js)](https://threejs.org/)
[![Platform](https://img.shields.io/badge/Full--Stack-Cross--Platform-blue?style=flat-square)]()
[![License](https://img.shields.io/badge/License-MIT-lightgrey?style=flat-square)](LICENSE)

An architectural, WebGL-powered 3D personal portfolio and interactive lab built with vanilla HTML5, CSS3, JavaScript (ES6+), and **Three.js**. The application immerses visitors in a spatial environment where skills, multi-target devices, projects, and contact endpoints can be navigated dynamically in 3D space. 

**Live Deployment:** [debbarmanshivam20-hue.github.io/Shivam3D_lab.com](https://debbarmanshivam20-hue.github.io/Shivam3D_lab.com/)

---

## Highlights & Features

* **Spatial Architectural Scene:** Built from scratch using Three.js primitive geometries, dynamic canvas textures, directional shadows, and physical materials.
* **Tween-Driven Waypoint Navigation:** Smooth camera choreographies between distinct stations (`Studio`, `About`, `Tech Lab`, `Cross-Platform`, `Projects`, `Physics`, and `Contact`) powered by `tween.js`.
* **3D Raycasting & Interactive Nodes:** Interactive meshes trigger slide-in glassmorphism inspect panels for technologies, projects, and external resources.
* **Cross-Platform Multi-Device Lab:** Real-time spatial representation of mobile, tablet, and desktop viewports demonstrating Flutter & Dart shared business logic with animated dashed buslines.
* **Hardware Fallbacks & Adaptive Viewport:** Full graceful degradation overlay for browsers or hardware configurations without WebGL support, plus mobile-responsive HUD controls.
* **Hash-Based Deep Linking:** Supports URL hash routing (e.g. `#projects`, `#tech`, `#project=cafe`) for direct sharing.

---

## Tech Stack

* **Core Graphics & Math:** Three.js (r128), OrbitControls, Tween.js (v18.6.4)
* **Frontend Layer:** HTML5 Canvas, Vanilla ES6+ JavaScript, CSS Modern Glassmorphism
* **Typography:** Cinzel, Inter, JetBrains Mono (Google Fonts)
* **Core Disciplines Showcased:**
  * **Frontend / Full-Stack:** React.js, Redux Toolkit, Tailwind CSS, Node.js, Express.js, MongoDB, REST APIs
  * **Cross-Platform:** Flutter, Dart, Responsive Multi-Platform Layouts

---

## Project Structure

```text
.
├── index.html        # Single-file architecture containing UI, 3D Engine, and Data
└── README.md         # Documentation

```

All logic, styling, textures, and data models are unified in `index.html` for maximum portability, low latency, and zero-build GitHub Pages deployment.

---

## Portfolio Data Configuration

To personalize your portfolio information, links, and backend form integration, update the central `portfolioData` object inside the `<script>` tag of `index.html`:

```javascript
const portfolioData = {
    profile: {
        name: "SHIVAM DEB BARMAN",
        title: "FULL-STACK & CROSS-PLATFORM DEVELOPER",
        location: "Kolkata, West Bengal, India",
        resumeUrl: "[https://your-resume-link.pdf](https://your-resume-link.pdf)" // Add direct resume URL here
    },
    // Customize your live project links
    projects: [
        {
            id: "cafe",
            liveUrl: "[https://your-cafe-demo.com](https://your-cafe-demo.com)",
            sourceUrl: "[https://github.com/yourusername/cafe-app](https://github.com/yourusername/cafe-app)"
        },
        // ...
    ],
    // Setup contact endpoints & social profiles
    contact: {
        email: "your.email@example.com",
        github: "[https://github.com/debbarmanshivam20-hue](https://github.com/debbarmanshivam20-hue)",
        linkedin: "[https://linkedin.com/in/yourprofile](https://linkedin.com/in/yourprofile)",
        config: {
            endpoint: "[https://formspree.io/f/your_form_id](https://formspree.io/f/your_form_id)", // Paste Formspree/backend endpoint
            method: "POST"
        }
    }
};

```

---

## Local Development & Setup

Because the project relies on WebGL and standard browser canvas security models, running it via a local static HTTP server is recommended:

1. **Clone the repository:**
```bash
git clone [https://github.com/debbarmanshivam20-hue/Shivam3D_lab.com.git](https://github.com/debbarmanshivam20-hue/Shivam3D_lab.com.git)
cd Shivam3D_lab.com

```


2. **Start a local development server:**
* Using Python 3:
```bash
python3 -m http.server 8000

```


* Using Node.js (`npx serve`):
```bash
npx serve .

```


* Or open directly with the **Live Server** extension in VS Code.


3. **Open in browser:**
```text
http://localhost:8000

```



---

## Navigation & Controls

| Input | Action |
| --- | --- |
| **Left Click + Drag** | Orbit / Rotate camera |
| **Right Click + Drag** | Pan scene camera |
| **Scroll Wheel** | Zoom in / out |
| **Left Click on Meshes** | Inspect technology, open project detail, or launch panel |
| **`Esc`** | Close active overlay panel and restore camera viewpoint |
| **`↑` / `↓` or `PgUp` / `PgDn**` | Cycle sequentially through architectural stations |
| **`Home` / `End**` | Jump to `Studio` / `Contact` |

---

## License

This project is licensed under the [MIT License](https://www.google.com/search?q=LICENSE).

```

```
