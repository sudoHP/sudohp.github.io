# sudoHP Software Studio — Public Web Portal

Welcome to the central public web portal for all iOS & iPadOS applications developed by **sudoHP**, published live at **[https://sudohp.github.io/](https://sudohp.github.io/)**.

This repository serves as the unified App Store compliance, privacy, terms, and customer support hub for all current and upcoming studio applications.

---

## 📱 Applications

### 🦘 Kangaroo Math Prep (iOS & iPadOS)
An independent, kid-friendly competition preparation tool featuring 1,000 algorithmic & verified math problems across Grades 1 through 8, official contest scoring, Apple Pencil scratchpad, and encouraging mascot companions.

* **App Overview & Portal**: [https://sudohp.github.io/kangaroo/](https://sudohp.github.io/kangaroo/)
* **Privacy Policy (COPPA & Kids Category Compliant)**: [https://sudohp.github.io/kangaroo/privacy](https://sudohp.github.io/kangaroo/privacy)
* **Terms of Service & Nominative Fair Use Disclaimers**: [https://sudohp.github.io/kangaroo/terms](https://sudohp.github.io/kangaroo/terms)
* **Customer Support & FAQ**: [https://sudohp.github.io/kangaroo/support](https://sudohp.github.io/kangaroo/support)
* **App Codebase Repository**: [https://github.com/sudoHP/kangaroo-math-app](https://github.com/sudoHP/kangaroo-math-app)

---

## 🏛️ Architecture: Multi-App Clean Routing

To ensure human-friendly URLs and compatibility with Apple App Store guidelines without exposing ugly `.html` extensions, every route uses directory-based `index.html` files:

```text
sudohp.github.io/
├── index.html                   → https://sudohp.github.io/ (Studio Hub)
├── kangaroo/
│   ├── index.html               → https://sudohp.github.io/kangaroo/ (App Home)
│   ├── privacy/
│   │   └── index.html           → https://sudohp.github.io/kangaroo/privacy (Privacy)
│   ├── terms/
│   │   └── index.html           → https://sudohp.github.io/kangaroo/terms (Terms)
│   └── support/
│       └── index.html           → https://sudohp.github.io/kangaroo/support (Support)
└── <future-app>/
    ├── index.html               → https://sudohp.github.io/<future-app>/
    ├── privacy/index.html       → https://sudohp.github.io/<future-app>/privacy
    └── support/index.html       → https://sudohp.github.io/<future-app>/support
```

---

## 🚀 Adding Future Applications

When launching a new app:
1. Create a folder in root named after the app slug (e.g. `quiz-master/`).
2. Add `index.html`, `privacy/index.html`, `terms/index.html`, and `support/index.html`.
3. Add a card to the Studio root [`index.html`](file:///Users/hp/AIProjects/sudohp.github.io/index.html).
4. Commit and push to `main` — GitHub Pages instantly deploys the new endpoints.

---

## 🔒 Privacy & Compliance Commitments

All sudoHP educational applications are built with strict adherence to:
* **COPPA (Children's Online Privacy Protection Act)**: Zero PII collected, zero user accounts, zero device tracking.
* **Apple Kids Category Guidelines (1.3 & 5.1.4)**: Zero third-party advertising SDKs, zero behavioral trackers, and interactive parental verification gates protecting external links and data resets.
* **Nominative Fair Use**: Independent educational practice with explicit trademark disclaimers.

---

## 📬 Contact & Inquiries

* **Developer Portal**: [https://sudohp.github.io/](https://sudohp.github.io/)
* **Support Email**: [support@mathkangarooprep.org](mailto:support@mathkangarooprep.org) *(Configurable to studio email)*
* **Issue Tracker**: [GitHub Issues](https://github.com/sudoHP/sudohp.github.io/issues)
