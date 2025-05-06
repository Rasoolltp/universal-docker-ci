# 🌐 Universal GitLab CI/CD Pipeline for Docker Projects

This repository provides a plug-and-play `.gitlab-ci.yml` file that you can add to **any project with a Dockerfile** to fully automate the CI/CD process — from build to deploy.

---

## 🚀 Features

- ✅ Auto-detects if a `Dockerfile` exists
- 🔧 Runs language-specific build steps (Laravel, Go, .NET, etc.)
- 🐳 Builds Docker image
- 📤 Pushes image to GitLab Container Registry
- 📦 Deploys to your target server over SSH

---

## 📁 How to Use

### 1. Add `.gitlab-ci.yml` to your project's root

Copy the `gitlab-ci.yml` from this repo into your project.

```bash
curl -O https://raw.githubusercontent.com/<your-username>/universal-docker-ci/main/gitlab-ci.yml


```yaml
include:
  remote: 'https://raw.githubusercontent.com/YOUR_USERNAME/universal-docker-ci/master/.gitlab-ci.yml'
