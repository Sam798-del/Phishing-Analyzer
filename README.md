# 🛡️ PhishGuard — Real-Time Phishing Threat Analyzer

[![Live Demo](https://img.shields.io/badge/Live_Demo-Online-brightgreen?style=for-the-badge&logo=githubpages&logoColor=white)](https://sam798-del.github.io/Phishing-Analyzer/)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

A lightweight, 100% client-side web application built using **HTML5, Vanilla CSS3, and JavaScript (ES6)** to analyze URLs, domain typosquatting vectors, and email text against real-time heuristic security algorithms.

👉 **[Click Here to Test the Live Application](https://sam798-del.github.io/Phishing-Analyzer/)**

---

## 📌 Project Summary

Modern phishing attacks often bypass traditional static blacklists through short-lived domains and subtle typosquatting. **PhishGuard** evaluates target URLs and suspicious email text locally inside the browser using sub-5ms heuristic checks, providing instant risk scoring, structural breakdown chips, and clear mitigation feedback.

---

## ✨ Key Features

- **⚡ Instant Sub-5ms Client-Side Processing**: Operates entirely in the browser using zero external dependencies or server latency.
- **📊 Dynamic Circular Risk Meter**: Animates an interactive SVG gauge ring based on the calculated threat score (0 to 100).
- **🔗 Structural URL Parser Chips**: Deconstructs input strings into `Protocol`, `Hostname`, `TLD`, and `Character Length`.
- **⚠️ Heuristic Threat Flag Accordion**: Categorizes security triggers into `Critical`, `Warning`, and `Safe` indicators.
- **🎨 Cyberpunk Glassmorphism UI**: High-contrast dark theme designed with responsive CSS Grid and Flexbox layouts.

---

## ⚡ Technical & DSA Architecture

PhishGuard employs 5 heuristic analysis vectors to score incoming targets:

| Heuristic Vector | Detection Logic | 
| :--- | :--- | 
| **1. Protocol Verification** | Checks for unencrypted `http://` vs secure `https://` |
| **2. Numeric IP Hostname** | RegEx pattern matching (`/\b\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}\b/`) |
| **3. High-Risk TLD Check** | Set lookup against abuse-prone extensions (`.xyz`, `.top`, `.free`) | 
| **4. Typosquatting / Character Swap** | Substring Homoglyph matching (`paypa1`, `g00gle`, `arnazon`) |
| **5. Social Engineering Urgency** | Text array parsing for psychological pressure keywords | 

---

## 🛠️ Technology Stack

- **Structure**: HTML5 (Semantic elements, SVG Graphics)
- **Styling**: Vanilla CSS3 (CSS Variables, Flexbox, CSS Grid, Glassmorphism Backdrop Filters)
- **Logic**: Modern JavaScript ES6+ (Native `URL` API, DOM Manipulation, RegEx Engine)

---

## 🚀 How to Run Locally

Since PhishGuard is built as a pure frontend web application, **no server setup, Python, or Node.js installation is required**.

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Sam798-del/Phishing-Analyzer.git
   ```
2. **Launch in Browser**:
   - Double-click `index.html` to open it directly in Chrome, Edge, Firefox, or Safari!
   - Alternatively, open with VS Code **Live Server**.

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
