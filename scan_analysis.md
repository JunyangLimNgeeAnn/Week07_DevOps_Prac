# Security Scan Analysis - [5/12/2025]

## DAST Results (ZAP Baseline)
- Total URLs scanned: 45
- PASS: Y checks
- WARN-NEW: 3 warnings
- FAIL-NEW: 0 failures

### Warning Summary
The response does not protect against 'ClickJacking' attacks. It should include either Content-Security-Policy with 'frame-ancestors' directive or X-Frame-Options.

The site is only served under HTTP and not HTTPS.

Content Security Policy (CSP) is an added layer of security that helps to detect and mitigate certain types of attacks, including Cross Site Scripting (XSS) and data injection attacks. These attacks are used for everything from data theft to site defacement or distribution of malware. CSP provides a set of standard HTTP headers that allow website owners to declare approved sources of content that browsers should be allowed to load on that page — covered types are JavaScript, CSS, HTML frames, fonts, images and embeddable objects such as Java applets, ActiveX, audio and video files.


## SCA Results (Dependency Check)
- High severity: 0
- Medium severity: 0
- Low severity: 0
- 

### Vulnerable Packages
No vulnerable packages

## SAST Results (CodeQL)
- Total issues: 1
- By type: High

Running a Flask application with debug mode enabled may allow an attacker to gain access through the Werkzeug debugger.



## Recommendations
Ensure that Flask applications that are run in a production environment have debugging disabled.

