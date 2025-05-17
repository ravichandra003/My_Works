# QUESTIONS

## What is a JWT Token?
JWT (JSON Web Token) is a compact, URL-safe token format used for securely transmitting information between parties.  
It consists of three parts: `Header.Payload.Signature` and is commonly used in authentication systems.

## What are all security headers in HTTP methods and the relative attacks they can prevent?

| Security Header                 | Purpose                                                  | Attacks Prevented                          |
|--------------------------------|-----------------------------------------------------------|--------------------------------------------|
| `Content-Security-Policy`      | Restricts sources of scripts, styles, media, etc.         | Cross-Site Scripting (XSS)                 |
| `Strict-Transport-Security`    | Enforces HTTPS connections only                          | Man-in-the-Middle (MITM) Attacks           |
| `X-Frame-Options`              | Prevents embedding site in iframes                        | Clickjacking                               |
| `X-Content-Type-Options`       | Prevents MIME-type sniffing by the browser                | MIME-based attacks                         |
| `Referrer-Policy`              | Controls what information is sent in the `Referer` header | Information leakage                        |
| `Permissions-Policy`           | Limits use of browser features (e.g., mic, camera)        | Abuse of features, privacy breaches        |
| `X-XSS-Protection`             | Enables basic XSS filtering (legacy browsers)             | Basic Cross-Site Scripting (XSS) filtering |

---

# GOALS✅

- ❌ Enable HTTPS traffic on Burp Suite and explore different kinds of web traffic  
- ❌ Setup an Active Directory (AD) server for lab practice  
- ❌ Make notes for some processes:
  - SSH connection (all methods)
  - SCP (Secure Copy Protocol)
- ❌ Explore UFW (Uncomplicated Firewall) in Linux  
- ❌ Understand and document:
  - MITRE ATT&CK Framework
  - Cyber Kill Chain Model
- ❌ Learn scripting (Bash, PowerShell, Python) for automating analysis and detection
