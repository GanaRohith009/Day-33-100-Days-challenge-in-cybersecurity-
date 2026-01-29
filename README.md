# Day-33-100-Days-challenge-in-cybersecurity-
# Day 33: CSP Bypass Techniques

## 🎯 Objective
To understand how misconfigured Content Security Policy (CSP) headers can be bypassed by attackers to execute malicious scripts (XSS).

## 📝 Key Concepts

### 1. What is CSP?
Content Security Policy is an HTTP response header that allows site administrators to declare approved sources of content that browsers are allowed to load on that page.

### 2. Common Bypass Vectors
| Method | Description | Risk Level |
| :--- | :--- | :--- |
| **Unsafe-Inline** | Allows execution of inline scripts and styles. | High |
| **JSONP Endpoints** | Bypassing CSP by calling JSONP APIs on trusted domains. | Medium |
| **Wildcard Domains** | Using `*` in the source list, allowing any subdomain to host scripts. | High |
| **Clickjacking** | If `frame-ancestors` is missing or weak. | Medium |

## 🛠️ Lab Activity
- Analyzed various CSP configurations using **Google CSP Evaluator**.
- Practiced bypassing a weak CSP in a lab environment using a trusted CDN endpoint.
- Identified the difference between `nonce-based` and `whitelist-based` policies.

## 💡 Reflection
A "VIP Guest List" (CSP) is useless if the list says "Anyone from the internet is allowed." Moving forward, I will focus on implementing **Strict CSP** using nonces or hashes.

---
[<- Previous Day](Day32.md) | [Next Day ->](Day34.md)
