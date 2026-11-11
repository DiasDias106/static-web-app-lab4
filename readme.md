# ☁️ Azure Static Web Apps: Lab 4

<p>
  <img src="https://img.shields.io/badge/Azure-Static%20Web%20Apps-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" alt="Azure Static Web Apps"/>
  <img src="https://img.shields.io/badge/GitHub%20Actions-CI%2FCD-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
</p>

A hands-on cloud lab for deploying a vanilla HTML/CSS/JavaScript site to **[Azure Static Web Apps](https://learn.microsoft.com/azure/static-web-apps/overview)** with an automated **GitHub Actions** pipeline. It is based on Microsoft's *Vanilla JavaScript* starter template.

## 🎯 What this lab covers

- Creating an **Azure Static Web App** resource connected to a GitHub repository
- **CI/CD with GitHub Actions**: every push to `main` builds and deploys the site, and pull requests get preview environments that close automatically
- Storing the deployment token safely as a **GitHub secret** (`AZURE_STATIC_WEB_APPS_API_TOKEN_*`)
- Using a **Dev Container** for a reproducible development environment

## 🚀 Run locally

```bash
git clone https://github.com/DiasDias106/static-web-app-lab4.git
cd static-web-app-lab4
npm install
npm start          # serves ./src on http://localhost:8000
```

Or open the repository in **GitHub Codespaces** / **VS Code Dev Containers**, which have all dependencies pre-installed.

## 📁 Structure

```
.
├── src/                    # Static site (index.html, styles.css)
├── .github/workflows/      # Azure Static Web Apps deployment pipeline
├── .devcontainer/          # Dev Container configuration
└── package.json            # Local dev server (sirv)
```
