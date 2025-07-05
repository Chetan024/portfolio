# 🌐 Portfolio Deployment with AWS 

This project automates the deployment of a static portfolio website using:
- **Amazon S3** for static file storage and hosting
- **Amazon CloudFront** for global content delivery and HTTPS
- **Amazon Route 53** for custom domain DNS
- **GitHub Actions** for continuous deployment from a GitHub repo

> ⚡️ Live at: [https://chetansoni.tech](https://chetansoni.tech)

---

## 🚀 Features

- ⚙️ Automated CI/CD via GitHub Actions
- 🌍 Custom domain with SSL (HTTPS)
- 🌐 CDN-backed performance using CloudFront
- 📁 Easy to update: push to GitHub → auto-deploys to AWS

---

## 🧱 Architecture

```mermaid
graph TD
    A["Developer pushes to GitHub"] --> B["GitHub Actions CI/CD"];
    B --> C["Upload files to S3 Bucket"];
    B --> D["Trigger CloudFront Invalidation"];
    C --> E["CloudFront Distribution"];
    E --> F["User Browser"];

    style A fill:#2e2e2e,stroke:#aaaaaa,stroke-width:1px,color:#ffffff
    style B fill:#264d73,stroke:#7ab8ff,stroke-width:1px,color:#ffffff
    style C fill:#2d7032,stroke:#8de98d,stroke-width:1px,color:#ffffff
    style D fill:#802828,stroke:#ff9999,stroke-width:1px,color:#ffffff
    style E fill:#6c2980,stroke:#ddaaff,stroke-width:1px,color:#ffffff
    style F fill:#2e2e2e,stroke:#aaaaaa,stroke-width:1px,color:#ffffff
```
---

## 📂 Project Structure

```
.
├── index.html
├── styles.css
├── script.js
├── assets/
├── .github/
│   ├── workflow/
│   │   ├── main.yml
└── README.md
```

