## 1. How we'll configure GitHub Actions

- Create a config file at `.github/workflows/checks.yml`
    - Set trigger
    - Add steps for running testing and linting

- Configure Docker Hub Auth

## 2. Docker Hub

- Need to pull base images
- Rate limits
    - Anonymous: 100/6h
    - Authenticated: 200/6h
- GitHub Actions uses shared IP addresses
    - Limit applied to all users
- Authenticate with Docker Hub
    - 200 pulls per 6h all to ourselves!

## 3. GitHub Token 관련
- https://limm-jk.tistory.com/11