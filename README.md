# Personal Profile Card — ApnoAI Task 2

A modern, responsive, and interactive Personal Profile Card built with **React 18** and **Tailwind CSS**, featuring glassmorphism design, real-time dark/light theme switching, dynamic skill badges, and interactive state management.

Developed as part of the **ApnoAI Internship — Task 2**.

---

## 🌐 Live Demo

Experience the live application deployed on Vercel:

🔗 **[https://my-profile-card-swart.vercel.app](https://my-profile-card-swart.vercel.app)**

---

## ✨ Features

- **Modern Glassmorphism UI**: Multi-layered frosted glass aesthetic with `backdrop-filter: blur(24px)`, subtle inner specular highlights, and ambient floating background gradient orbs that simulate authentic optical refraction.
- **Reusable React Component Architecture**: Powered by a modular `ProfileCard` component that accepts standard props (`name`, `role`, `bio`, `skills`, `avatar`, `github`, `twitter`, `linkedin`).
- **Interactive Dark / Light Mode Toggle**: Smooth theme switching using React `useState`:
  - **Light Mode**: Vibrant purple, pink, and orange gradient background with frosted white glass accents.
  - **Dark Mode**: Sleek dark slate/gray background with ambient violet and purple glowing accents.
  - Floating top-right toggle button featuring animated SVG Sun and Moon icons with contextual tooltips.
- **Interactive Connect Button**: State-managed connection button toggling between `"Connect"` and `"✓ Connected"` (transitions to a vibrant green state upon connection).
- **Dynamic Skills Badges**: Dynamically maps through the skills array using JavaScript `.map()`, rendering responsive pill badges with subtle hover elevation effects.
- **Social Media Links**: Circular SVG buttons for GitHub, Twitter / X, and LinkedIn that adapt to active themes and open securely in new tabs (`target="_blank" rel="noopener noreferrer"`).
- **Profile Avatar**: Circular avatar with an ambient border glow, smooth hover zoom and rotation animations, verified profile badge, and alt text mapped directly to the user's name.
- **Fully Responsive Layout**: Mobile-first design that fits smoothly across mobile phones, tablets, and desktop displays without horizontal scrolling.
- **Zero-Build Lightweight Execution**: Runs directly in the browser via React 18 UMD CDN and Babel Standalone for instant loading without mandatory bundler overhead.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **HTML5** | Semantic document structure |
| **React 18 (UMD CDN)** | Component-based UI and reactive state (`useState`) |
| **ReactDOM 18 (`createRoot`)** | Root rendering into the DOM |
| **Babel Standalone** | In-browser JSX transformation |
| **Tailwind CSS (CDN)** | Utility-first styling with runtime theme and keyframe configuration |
| **Google Fonts (Plus Jakarta Sans)** | Clean, modern typography |
| **Inline SVGs** | Sharp vector icons for social media, themes, and interactive states |
| **Vercel** | Production hosting and global edge deployment |

---

## 📁 Project Structure

```text
my-profile-card/
├── index.html              # Main single-page application (React 18 + Tailwind CSS + Babel)
├── profile image.jpeg      # Profile photo
└── README.md               # Project documentation
```

---

## 🚀 Getting Started / Local Setup

Because this project is built using React 18 via CDN and Babel Standalone, it requires zero build steps or package installations.

### Option 1: Direct File Opening
1. Clone the repository:
   ```bash
   git clone https://github.com/Shubhamkale5692/my-profile-card.git
   cd my-profile-card
   ```
2. Double-click `index.html` to open it in your preferred web browser (Chrome, Edge, Firefox, Brave, Safari).

### Option 2: Local HTTP Server (Recommended)
Using a lightweight local server ensures optimal resource loading:

- **Using VS Code Live Server**:
  Right-click `index.html` in VS Code and select **"Open with Live Server"**.

- **Using Node.js (`npx serve`)**:
  ```bash
  npx serve .
  ```

- **Using Python**:
  ```bash
  # Python 3
  python -m http.server 3000
  ```
  Then open `http://localhost:3000` in your browser.

---

## ⚙️ Customization Guide

All personal profile information is centralized inside `index.html` under the `studentProfileData` configuration object:

```javascript
const studentProfileData = {
  name: "Shubham Kale",
  role: "Full-Stack Developer",
  bio: "I'm an aspiring Full-Stack Developer passionate about building modern, responsive, and user-friendly web applications. I'm also interested in exploring Web3 technologies and blockchain development.",
  skills: ["React.js", "JavaScript", "HTML5", "CSS3", "Node.js", "Git", "GitHub"],
  avatar: "profile image.jpeg",
  github: "https://github.com/Shubhamkale5692",
  twitter: "https://x.com/Shubham_5692",
  linkedin: "https://www.linkedin.com/in/shubham-kale-162a23322"
};
```

Update any of these fields to immediately reflect your information on the profile card.

---

## 👨‍💻 Author

**Shubham Kale**
- **GitHub**: [@Shubhamkale5692](https://github.com/Shubhamkale5692)
- **LinkedIn**: [Shubham Kale](https://www.linkedin.com/in/shubham-kale-162a23322)
- **Twitter / X**: [@Shubham_5692](https://x.com/Shubham_5692)

---

## 📜 Acknowledgements & Task Credit

- **Organization**: ApnoAI
- **Internship Program**: ApnoAI Internship
- **Assignment**: Task 2 — Personal Profile Card Website
- **Footer Attribution**: `"Built with React 18 + Tailwind CSS · ApnoAI Task 2"`
