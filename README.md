# Universal Docker CI Pipeline

This repository contains a universal GitLab CI pipeline configuration (`.gitlab-ci.yml`) that works with any project that includes a `Dockerfile`. The pipeline will automatically build and push Docker images to GitLab's container registry.

## Usage

To use this CI pipeline in your GitLab project, follow these steps:

1. **Create a new GitLab project** or use an existing one.
2. **Add your Dockerfile** to the project.
3. **Add the `.gitlab-ci.yml` file** from this repository to your GitLab project by including it via remote:

```yaml
include:
  remote: 'https://raw.githubusercontent.com/YOUR_USERNAME/universal-docker-ci/master/.gitlab-ci.yml'
