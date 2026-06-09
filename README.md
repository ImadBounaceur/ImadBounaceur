<h1 align="center">Hi, I'm Imad 👋</h1>

<p align="center">
  <b>MSc Cybersecurity · Behavioural Authentication Research · Identity & Access Management</b><br/>
  <i>University of Essex</i>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/imad-bounaceur-a7b26a261">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white"/>
  </a>
  <a href="mailto:bounaceur.imad19@email.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white"/>
  </a>
  <img src="https://komarev.com/ghpvc/?username=ImadBounaceur&color=6366f1&style=flat&label=Profile+views"/>
</p>
---

## About me

MSc Cybersecurity student at the University of Essex, specialising in **Identity and Access Management (IAM)**. My dissertation focuses on continuous behavioural authentication — building a system that silently verifies users through how they type and move their mouse, rather than relying on one-time password checks.

- 🎓 MSc Cybersecurity — University of Essex (2025)
- 🔬 Dissertation: Continuous behavioural authentication using keystroke & mouse biometrics
- 🎯 Career focus: Identity & Access Management (IAM), Zero Trust architecture
- 🌍 London, UK

---

## Dissertation project — OmniAuth

> A cross-platform continuous behavioural authentication system built for real-world IAM deployment.

**Core idea:** Instead of asking "who are you?" once at login, the system continuously asks "does this still behave like you?" — scoring trust from 0–100 in real time and responding proportionally.

**How it works:**

- Captures **30 biometric features** in real time — 16 keystroke (dwell, flight, digraph latency, rhythm patterns) and 14 mouse (speed, trajectory, idle ratio, click intervals), grounded in Dr. Buriro's published F-type taxonomy
- Runs a **three-model ML ensemble** — One-Class SVM, Isolation Forest, and LSTM Autoencoder — each trained exclusively on the enrolled user's own behavioural profile (one-class classification)
- Outputs a **trust score (0–100)** via threshold-anchored sigmoid mapping, triggering graduated responses: silent monitoring → step-up MFA → session lock
- IAM layer: **Zero Trust policy engine**, RBAC tied to trust score thresholds, OAuth 2.0/OIDC via **Keycloak**, structured JSON audit logging, GDPR documentation

**Architecture:**

```
Electron desktop (biometric capture: keyboard + touchpad WM_POINTER)
        │
        ▼
Flask REST API  ──►  ML ensemble (SVM + IForest + LSTM)  ──►  Trust score
        │
        ▼
Keycloak OIDC  ──►  Zero Trust engine  ──►  RBAC enforcement
```

**Stack:**

![Python](https://img.shields.io/badge/Python_3.11-3776AB?style=flat&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Electron](https://img.shields.io/badge/Electron-47848F?style=flat&logo=electron&logoColor=white)
![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?style=flat&logo=keycloak&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

---

## Other projects

Earlier work from my undergraduate years — full-stack Rails applications:

| Project | Description | Stack |
|---------|-------------|-------|
| [🛖 Virtual Cafe](https://github.com/ImadBounaceur/Virtual-Cafe) | Online café ordering system | Rails, JS, PostgreSQL |
| [🧩 Escape Room](https://github.com/ImadBounaceur/Escape-Room) | Browser-based interactive puzzle game | Rails, CSS, JS |

---

## Skills

**Security & IAM**

![Zero Trust](https://img.shields.io/badge/Zero_Trust-Architecture-333?style=flat)
![OAuth2](https://img.shields.io/badge/OAuth_2.0-4285F4?style=flat&logo=google&logoColor=white)
![OIDC](https://img.shields.io/badge/OIDC-Keycloak-4D4D4D?style=flat)
![RBAC](https://img.shields.io/badge/RBAC-Policy_Engine-555?style=flat)
![GDPR](https://img.shields.io/badge/GDPR-Compliance-003366?style=flat)

**ML & Data**

![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)

**Dev & Infrastructure**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white)
![Electron](https://img.shields.io/badge/Electron-47848F?style=flat&logo=electron&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Ruby on Rails](https://img.shields.io/badge/Rails-CC0000?style=flat&logo=ruby-on-rails&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)

---

## GitHub stats

<p align="center">
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=ImadBounaceur&show_icons=true&theme=tokyonight&hide_border=true&count_private=true"/>
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ImadBounaceur&layout=compact&theme=tokyonight&hide_border=true"/>
</p>

---

<p align="center">
  <i>Open to IAM and security engineering roles — feel free to reach out</i>
</p>
