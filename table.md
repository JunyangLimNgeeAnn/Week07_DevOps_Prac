# Security Findings



The following WARN-NEW issues were identified by the ZAP scan:

| Code   | Issue                                  | Risk Level | Affected URL | Why It Matters                                                                                  |
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 10038  | Content Security Policy (CSP) Header Not Set | Medium     | http://localhost:5000 | CSP helps prevent XSS and data injection attacks by controlling which sources of content the browser can load. |
| 10106  | HTTP Only Site                          | Medium     | http://localhost:5000 | The site is served only over HTTP, so traffic is unencrypted and can be intercepted by attackers. |
| 10020  | Missing Anti-clickjacking Header        | Medium     | http://localhost:5000 | Prevents clickjacking attacks by ensuring pages cannot be framed by malicious sites.          |
