# AuthGate Slides

Presentation slides for **AuthGate** — introducing how a lightweight **Identity Gateway** can unify OAuth / OIDC authentication and JWT issuance.

## 🔗 Live Demo

**https://go-authgate.github.io/slides/**

## 📑 Overview

The slides cover the following topics:

- **Three Pain Points** — why a unified identity gateway is needed
- **What is AuthGate** — a lightweight Identity Gateway
- **Three OAuth Flows** — Auth Code + PKCE, covering browser, CLI/IoT, and service-to-service clients
- **Which Flow When** — choosing the right flow for Web / SPA / Mobile
- **Token Design** — access and refresh tokens stored together, `token_category`, and revocation
- **Resource Server Validation** — `aud` audience binding and multi-API isolation (api-a.corp / api-b.corp)
- **Observability** — metrics such as `auth_login_total`, `http_request_duration`, and audit events

Speaker: **appleboy**

## 🚀 Local Preview

The slides are a single self-contained `index.html` file (all assets are inlined). Just open it in a browser:

```bash
open index.html
```

Or serve it with a local HTTP server:

```bash
python3 -m http.server 8080
# open http://localhost:8080
```

## 📦 Deployment

The slides are deployed via **GitHub Pages** from the root of the `main` branch.
After updating the content, simply push to `main` and GitHub Pages will redeploy automatically:

```bash
git add index.html
git commit -m "Update slides"
git push origin main
```
