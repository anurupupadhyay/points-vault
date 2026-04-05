# Points Vault

Central platform to aggregate, track, and optimize credit card points and loyalty programs.

---

## 🌐 Live Environments

### Dev Web
- **URL:** https://dev.pointsvault.app
- **Stack:** CloudFront + S3 + HTTPS

### Auth (Cognito Hosted UI)
- **Auth Domain:** https://auth.dev.pointsvault.app
- **OAuth Flow:** Authorization Code Grant

---

## 🔐 Authentication (Cognito)

- **User Pool:** AWS Cognito (us-east-2)
- **Client ID:** `7184m0ppjiott8skj0vgltkerc`
- **Authorize URL:**
- https://auth.dev.pointsvault.app/oauth2/authorize

- **Working Redirect (Dev):**

https://dev.pointsvault.app/?code=...

✅ End-to-end login verified.

---

## 🧱 Infrastructure Overview

| Component        | Service        | Region      |
|------------------|----------------|-------------|
| DNS              | Cloudflare     | Global      |
| TLS Certs        | ACM            | us-east-1   |
| Frontend (Dev)   | S3 + CloudFront| Global      |
| Auth             | Cognito        | us-east-2   |
| IaC              | AWS CDK        | —           |

---

## 🚧 Current Status

- ✅ Dev infrastructure live
- ✅ Custom auth domain working
- ✅ OAuth flow validated
- 🚧 Token exchange + session handling next

---

## ▶️ Next Steps

- Exchange authorization code → tokens
- Replace placeholder with Next.js frontend
- Add API Gateway + Lambda (protected by Cognito)

---

_Last updated: April 2026_
