# Web Application Security Roadmap — Complete Beginner to Advanced

A TryHackMe-style, structured path covering everything from "what is HTTP" to expert-level exploitation, bug bounty, and certification. Structure: **Module (Heading) → Section (Subheading) → Topic (Sub-subheading/bullets)**. Modules are ordered so each one builds on the last.

---

## Module 1: Fundamentals

### 1.1 How the Web Works
- HTTP/HTTPS protocol basics
- Request/Response lifecycle
- URLs, URIs, and domains
- DNS resolution process
- TCP/IP and the network stack
- Client-server architecture
- Ports and protocols

### 1.2 HTTP Deep Dive
- HTTP methods
- HTTP headers (request & response)
- Request
    - GET → get data from server
    - POST → send data to server
    - PUT → replace existing data with new data
    - DELETE → removes specific data from server
    - PATCH → applies partial update
    - HEAD → same as GET but no body (metadata only)
    - OPTIONS → discover allowed methods on a resource
- Response
- Status codes
    - 1xx → informational
    - 2xx → success
    - 3xx → redirection
    - 4xx → client errors
    - 5xx → server errors
- HTTP/1.1 vs HTTP/2 vs HTTP/3
- Cookies and sessions
- Content-Type and MIME types
- Caching headers

### 1.3 Web Architecture
- Frontend vs backend
- Client-side vs server-side rendering
- MVC/MVT architecture
- Static vs dynamic content
- Load balancers, proxies, reverse proxies
- CDNs

### 1.4 Programming Foundations for Security
- HTML structure basics
- CSS basics relevant to security (clickjacking context)
- JavaScript fundamentals
- Server-side languages overview (PHP, Python, Node.js, Java)
- Databases (SQL vs NoSQL) basics
- Regular expressions basics (needed later for filter/WAF bypass)

### 1.5 Security Mindset
- CIA Triad (Confidentiality, Integrity, Availability)
- Threat modeling basics
- Attack surface concept
- Defense in depth
- Principle of least privilege
- Risk assessment basics

### 1.6 Setting Up a Lab
- Installing Burp Suite / OWASP ZAP
- Setting up vulnerable apps (DVWA, WebGoat, Juice Shop)
- Browser dev tools
- Virtual machines & Docker for labs
- Kali Linux basics
- Configuring FoxyProxy / browser proxy setup

---

## Module 2: Web Technologies & Stack

### 2.1 Frontend Technologies
- HTML5 security-relevant features
- CSS injection surface
- JavaScript engines and execution
- DOM structure and manipulation
- Single Page Applications (SPA)
- Frontend frameworks overview (React, Angular, Vue) — security implications

### 2.2 Backend Technologies
- Server-side frameworks overview (Express, Django, Spring, Laravel, .NET)
- Templating engines (Jinja2, EJS, Handlebars) & injection risks
- ORMs and query builders
- Server configuration basics (Apache, Nginx, IIS)

### 2.3 Data Formats
- JSON structure and parsing
- XML structure and parsing
- YAML basics
- Serialization/deserialization concepts

### 2.4 State Management
- Cookies (attributes, flags)
- Sessions (server-side)
- Tokens (JWT structure)
- Local storage / session storage
- State in SPAs

### 2.5 Web Communication Patterns
- REST APIs
- GraphQL basics
- WebSockets
- gRPC basics
- Webhooks
- Server-Sent Events

### 2.6 Databases
- SQL fundamentals
- NoSQL fundamentals (MongoDB, Redis)
- Database permissions model
- Stored procedures

### 2.7 Web Servers & Infrastructure
- Apache/Nginx configuration security
- Reverse proxy behavior
- Containers (Docker) basics
- Microservices architecture

---

## Module 3: Security Fundamentals

### 3.1 Core Security Principles
- Trust boundaries
- Input validation vs output encoding
- Allowlisting vs denylisting
- Fail-safe defaults
- Separation of duties

### 3.2 Cryptography Basics
- Symmetric vs asymmetric encryption
- Hashing algorithms (MD5, SHA family)
- Salting and peppering
- HMAC
- Digital signatures
- Certificate basics (SSL/TLS)
- Public Key Infrastructure (PKI)

### 3.3 TLS/SSL Security
- TLS handshake process
- Certificate validation
- Common TLS misconfigurations
- SSL stripping
- Certificate pinning

### 3.4 Encoding & Escaping
- URL encoding
- HTML entity encoding
- Base64 encoding
- Unicode normalization issues
- Encoding vs encryption vs hashing

### 3.5 Same-Origin Policy & CORS
- Origin concept
- Same-Origin Policy (SOP) rules
- CORS headers and mechanics
- CORS misconfigurations
- Cross-origin resource sharing pitfalls

### 3.6 Security Headers
- Content-Security-Policy (CSP)
- X-Frame-Options
- Strict-Transport-Security (HSTS)
- X-Content-Type-Options
- Referrer-Policy
- Permissions-Policy

### 3.7 Threat Actors & Motivations
- Script kiddies vs APTs
- Insider threats
- Hacktivism
- Financially motivated attacks
- Nation-state actors

### 3.8 Security Frameworks
- OWASP Top 10 (overview)
- OWASP ASVS
- NIST Cybersecurity Framework
- CWE/CVE systems
- CVSS scoring

---

## Module 4: Legal & Ethical Considerations

> Placed before any hands-on testing modules — know the rules before you touch a target.

### 4.1 Laws & Regulations
- Computer Fraud and Abuse Act (CFAA) and regional equivalents
- Data protection laws relevant to testing (GDPR context)

### 4.2 Responsible Disclosure
- Coordinated vulnerability disclosure process
- Safe harbor language in bug bounty programs
- Working within authorized scope only

### 4.3 Professional Ethics
- Client confidentiality
- Avoiding destructive testing
- Documentation and evidence handling

---

## Module 5: Core Web Vulnerabilities

### 5.1 Injection Vulnerabilities
- SQL Injection
    - Error-Based SQLi
    - UNION-Based SQLi
    - Blind SQLi (boolean-based, time-based)
    - Out-of-Band SQLi
    - Second-Order SQLi
- NoSQL Injection
    - Operator injection (MongoDB `$ne`, `$gt`)
    - Authentication bypass via NoSQLi
- Command Injection
    - Blind command injection
    - Out-of-band command injection (OAST)
- LDAP Injection
- XPath Injection
- Template Injection (SSTI)
    - Client-side template injection (CSTI)
- CRLF Injection / HTTP Response Splitting
- Header Injection
- HTTP Parameter Pollution (HPP)

### 5.2 Cross-Site Scripting (XSS)
- Reflected XSS
- Stored XSS
- DOM-based XSS
- Blind XSS
- Mutation XSS
- Self-XSS
- XSS filter evasion techniques
- CSP bypass techniques for XSS

### 5.3 Cross-Site Request Forgery (CSRF)
- CSRF fundamentals
- Token-based protection
- SameSite cookie protection
- CSRF in JSON APIs
- Login CSRF

### 5.4 Server-Side Request Forgery (SSRF)
- Basic SSRF
- Blind SSRF
- SSRF via file upload
- SSRF to cloud metadata endpoints
- SSRF filter bypass techniques
    - DNS rebinding
    - URL parser confusion / IP obfuscation

### 5.5 XML-Related Vulnerabilities
- XML External Entity (XXE)
- XML Bomb (Billion Laughs)
- SOAP injection
- Blind XXE (OOB exfiltration)

### 5.6 File-Related Vulnerabilities
- Unrestricted file upload
- Path traversal / directory traversal
- Local File Inclusion (LFI)
- Remote File Inclusion (RFI)
- Zip slip vulnerability
- PHP wrapper abuse (php://filter, data://, phar://)

### 5.7 Deserialization Vulnerabilities
- Insecure deserialization concepts
- Java deserialization
- PHP object injection
- Python pickle vulnerabilities
- .NET deserialization (ViewState)

### 5.8 Business Logic Vulnerabilities
- Race conditions
- Price manipulation
- Workflow bypass
- Insufficient rate limiting
- Logic flaws in multi-step processes
- Coupon/promo abuse

### 5.9 Access Control Vulnerabilities
- Insecure Direct Object Reference (IDOR)
- Broken Object Level Authorization (BOLA)
- Privilege escalation (horizontal/vertical)
- Forced browsing
- Missing function-level access control

### 5.10 Client-Side Vulnerabilities
- Clickjacking
- DOM clobbering
- Prototype pollution (client-side)
- Open redirects
- Tabnabbing
- postMessage vulnerabilities
- Client-side path traversal

### 5.11 Information Disclosure
- Verbose error messages
- Directory listing
- Source code exposure
- Metadata leakage
- Debug mode exposure
- Comments/backup file leakage (.bak, .old, .git exposure)

### 5.12 Denial of Service
- Application-layer DoS
- ReDoS (Regex DoS)
- Resource exhaustion
- Algorithmic complexity attacks

### 5.13 Miscellaneous Vulnerabilities
- Host header injection
    - Password reset poisoning
- Cache poisoning
- Web cache deception
- HTTP request smuggling
    - CL.TE, TE.CL, TE.TE variants
- Subdomain takeover
- Mass assignment
- Prototype pollution (server-side, Node.js)

---

## Module 6: Authentication & Session Security

### 6.1 Authentication Fundamentals
- Authentication factors (something you know/have/are)
- Password-based authentication
- Multi-factor authentication (MFA)
- Password hashing best practices (bcrypt, Argon2)
- Password policies

### 6.2 Authentication Attacks
- Brute force attacks
- Credential stuffing
- Password spraying
- Account enumeration
- Session fixation
- Session hijacking

### 6.3 Session Management
- Session ID generation
- Session timeout policies
- Secure cookie flags (HttpOnly, Secure, SameSite)
- Session invalidation on logout

### 6.4 Modern Authentication Protocols
- OAuth 2.0 flow and grant types
- OpenID Connect (OIDC)
- SAML basics
- JWT structure and validation
- JWT vulnerabilities (alg confusion, weak secrets, kid injection)

### 6.5 Authorization Models
- Role-Based Access Control (RBAC)
- Attribute-Based Access Control (ABAC)
- Discretionary vs Mandatory Access Control
- Multi-tenancy authorization issues

### 6.6 Password Recovery & MFA Flaws
- Insecure password reset flows
- OTP bypass techniques
- MFA fatigue attacks
- Backup code weaknesses
- CAPTCHA bypass techniques

### 6.7 Single Sign-On (SSO) Security
- SSO architecture
- SAML vulnerabilities
- OAuth misconfigurations
- Token leakage in redirects

---

## Module 7: API Security

### 7.1 API Fundamentals
- REST API design principles
- GraphQL architecture
- API versioning
- API documentation risks (Swagger/OpenAPI exposure)

### 7.2 OWASP API Security Top 10
- Broken Object Level Authorization
- Broken Authentication
- Broken Object Property Level Authorization
- Unrestricted Resource Consumption
- Broken Function Level Authorization
- Unrestricted Access to Sensitive Business Flows
- Server-Side Request Forgery
- Security Misconfiguration
- Improper Inventory Management
- Unsafe Consumption of APIs

### 7.3 GraphQL-Specific Security
- Introspection abuse
- Query depth/complexity attacks
- Batching attacks
- Field-level authorization issues

### 7.4 API Authentication Mechanisms
- API keys
- OAuth for APIs
- Mutual TLS
- Rate limiting strategies

### 7.5 API Testing Techniques
- Fuzzing API endpoints
- Parameter tampering
- Mass assignment in APIs
- Testing hidden/undocumented endpoints

### 7.6 Microservices & API Gateway Security
- API gateway misconfigurations
- Service-to-service authentication
- Internal API exposure risks

---

## Module 8: Browser & Client-Side Security

### 8.1 Browser Security Model
- Same-Origin Policy deep dive
- Sandboxing concepts
- Process isolation
- Content Security Policy in depth

### 8.2 Browser-Based Attacks
- Clickjacking techniques
- UI redressing
- Browser extension vulnerabilities
- Man-in-the-Browser attacks

### 8.3 Cookies & Storage Security
- Cookie attributes deep dive
- LocalStorage vs SessionStorage risks
- IndexedDB security
- Third-party cookie issues

### 8.4 Modern Browser Security Features
- Subresource Integrity (SRI)
- Feature-Policy/Permissions-Policy
- Trusted Types
- Fetch metadata headers
- COOP/COEP/CORP headers

### 8.5 Web Workers & Service Workers
- Service worker security model
- Cache poisoning via service workers
- Web worker isolation

### 8.6 WebSocket Security
- Cross-Site WebSocket Hijacking (CSWSH)
- Origin validation for WebSockets
- WebSocket message fuzzing

---

## Module 9: Cloud & Modern Architecture Security

### 9.1 Cloud-Hosted Web App Risks
- Cloud storage misconfigurations exposing web app data (S3 buckets etc.)
- Cloud metadata service exploitation (via SSRF)
- IAM misconfigurations affecting web app access
- Multi-tenant web app isolation issues

### 9.2 Serverless Web Apps
- Function-as-a-Service (FaaS) backend risks
- Event injection in serverless web backends
- Serverless API misconfigurations

### 9.3 Modern Web App Architectures
- JAMstack security considerations
- Progressive Web Apps (PWA) security
- WebAssembly security basics
- Static site generator risks

### 9.4 Third-Party Integrations
- Third-party script/widget risks
- Dependency confusion in frontend packages
- Supply chain risks in npm/CDN-loaded libraries
- Web app secrets exposure (API keys in frontend code)

---

## Module 10: Secure Coding & SDLC

### 10.1 Secure Coding for Web Apps
- Input validation techniques (client-side & server-side)
- Output encoding techniques (context-aware encoding)
- Parameterized queries / prepared statements
- Secure error handling in web responses
- Secure logging practices (avoiding sensitive data leaks)

### 10.2 Secure Design Patterns for Web Apps
- Threat modeling a web application (data flow diagrams)
- Designing secure authentication flows
- Designing secure file upload handling
- Secure session design

### 10.3 Frontend Secure Coding
- Safe DOM manipulation practices
- Avoiding dangerous sinks (innerHTML, eval, etc.)
- Secure use of frontend frameworks (React/Angular/Vue escaping)
- Content Security Policy implementation

### 10.4 Backend Secure Coding
- Secure database access patterns
- Secure file handling on the server
- Secure API endpoint design
- Rate limiting and abuse prevention implementation

### 10.5 Secrets & Configuration in Web Apps
- Avoiding hardcoded secrets in code/config
- Environment variable best practices for web apps
- Secure handling of API keys in frontend vs backend

### 10.6 Code Review for Web App Security
- Manual secure code review checklist for web apps
- Static Application Security Testing (SAST) for web codebases
- Common vulnerable code patterns to spot in review

---

## Module 11: Tools of the Trade

### 11.1 Proxy & Interception Tools
- Burp Suite (Community & Pro features)
- OWASP ZAP
- Fiddler

### 11.2 Scanning Tools
- Nmap basics
- Nikto
- Nessus/OpenVAS overview
- SQLmap

### 11.3 Reconnaissance Tools
- Subdomain enumeration tools (Sublist3r, Amass, Subfinder)
- Google Dorking
- Shodan basics
- WHOIS and DNS recon tools
- Content discovery (ffuf, gobuster, feroxbuster)
- Historical URL discovery (Wayback Machine, gau, waybackurls)
- Live host probing (httpx)
- Vulnerability scanning automation (Nuclei)

### 11.4 Exploitation Frameworks
- Metasploit basics
- Custom exploit scripting

### 11.5 Static & Dynamic Analysis Tools
- SAST tools overview
- DAST tools overview
- IAST concepts

### 11.6 Browser-Based Tools
- Browser Developer Tools for security testing
- Extensions (Wappalyzer, EditThisCookie, etc.)

### 11.7 Scripting for Security
- Python for security automation
- Bash scripting basics for pentesting
- Writing custom fuzzers

---

## Module 12: Reconnaissance & Enumeration Methodology

### 12.1 Passive Recon
- OSINT gathering (WHOIS, certificate transparency logs)
- Google/Shodan/Censys dorking
- Wayback Machine mining for old endpoints

### 12.2 Active Recon
- Subdomain enumeration workflow (bruteforce + permutation + cert logs)
- Port scanning and service fingerprinting
- Technology stack fingerprinting (Wappalyzer, headers)

### 12.3 Content & Endpoint Discovery
- Directory and file bruteforcing
- Parameter discovery (Arjun, ParamSpider)
- Hidden API endpoint discovery
- JavaScript file analysis for secrets and endpoints

### 12.4 Wordlists & Automation
- Building custom wordlists
- SecLists usage
- Chaining recon tools into automated pipelines

---

## Module 13: WAF & Filter Evasion

### 13.1 Detecting Protections
- Identifying WAF presence and vendor
- Identifying rate-limiting and behavioral detection

### 13.2 Evasion Techniques
- Encoding-based bypass (double encoding, mixed case)
- Payload obfuscation techniques
- Chunked transfer encoding tricks
- HTTP request smuggling for filter bypass

### 13.3 Rate Limit & Bot Protection Bypass
- IP rotation considerations
- Header manipulation (X-Forwarded-For tricks)
- CAPTCHA-solving service awareness (conceptual, ethics)

---

## Module 14: Penetration Testing Methodology

### 14.1 Penetration Testing Fundamentals
- Testing types (black box, white box, grey box)
- Rules of engagement
- Scope definition

### 14.2 Testing Standards
- OWASP Testing Guide
- PTES (Penetration Testing Execution Standard)
- NIST 800-115

### 14.3 Reconnaissance Phase
- Passive information gathering
- Active information gathering
- OSINT techniques

### 14.4 Vulnerability Assessment
- Automated scanning approach
- Manual testing techniques
- False positive/negative analysis

### 14.5 Exploitation Phase
- Proof-of-concept development
- Privilege escalation testing
- Post-exploitation basics

### 14.6 Reporting
- Writing effective vulnerability reports
- CVSS scoring in reports
- Remediation recommendations
- Executive summary writing

### 14.7 Specialized Testing
- Mobile app backend testing basics
- API-specific test plans
- Cloud environment testing

---

## Module 15: Practice Labs & CTFs

### 15.1 Beginner Labs
- DVWA walkthroughs (low/medium security)
- bWAPP basics
- OWASP Juice Shop introductory challenges

### 15.2 Intermediate Labs
- PortSwigger Web Security Academy labs
- HackTheBox web challenges (easy/medium)
- TryHackMe web security rooms

### 15.3 Advanced Labs
- Juice Shop advanced challenges
- HackTheBox web challenges (hard/insane)
- Custom CTF-style challenges per vulnerability class

### 15.4 Real-World Case Studies
- Historical major breaches (analysis of root cause)
- Bug bounty writeups analysis
- CVE deep-dive case studies

### 15.5 Capstone Projects
- Full black-box assessment of a vulnerable app
- Build-and-break exercises (build a feature, then attack it)
- Bug bounty simulation exercise

### 15.6 Certification-Aligned Practice
- OSCP-style exercises
- eWPT/eWPTX-style web challenges
- CEH-aligned practice questions

---

## Module 16: Bug Bounty & Career Path

### 16.1 Bug Bounty Platforms
- HackerOne, Bugcrowd, Intigriti overview
- Program scope and policy reading
- Choosing targets as a beginner

### 16.2 Bug Hunting Methodology
- Recon-driven hunting workflow
- Note-taking and target tracking
- Duplicate/triage awareness

### 16.3 Reporting & Communication
- Writing a clear, reproducible bug bounty report
- Impact articulation for triagers
- Handling disputes and re-testing

### 16.4 Building a Career
- Building a public portfolio (write-ups, GitHub, blog)
- Resume/CV tips for AppSec/pentest roles
- Interview preparation for web security roles

---

## Module 17: Continuous Learning & Community

### 17.1 Staying Current
- Following security researchers and disclosures
- Reading CVE advisories relevant to web tech
- Subscribing to security newsletters

### 17.2 Community Engagement
- Security conferences (DEF CON, Black Hat, BSides, local meetups)
- CTF communities and teams
- Contributing write-ups back to the community

---

## Module 18: Certifications for Web Application Security

> Certifications validate the skills built across this roadmap. Listed in the order most people pursue them, beginner to expert.

### 18.1 Foundational / General Cybersecurity (optional starting point)
- CompTIA Security+ — broad security fundamentals, not web-specific but a common first cert
- Google Cybersecurity Certificate — entry-level awareness certificate
- eJPT (eLearnSecurity Junior Penetration Tester) — beginner-friendly practical pentesting intro
- CC (ISC2 Certified in Cybersecurity) — free entry-level credential

### 18.2 Entry-Level Web Application Security
- eWPT (eLearnSecurity/INE Web Application Penetration Tester)
- CBBH (HTB Certified Bug Bounty Hunter)
- CAP (HTB Certified AppSec Practitioner)
- CEH (Certified Ethical Hacker) — broad, often required for compliance/HR filters

### 18.3 Intermediate-Level Web Application Security
- PortSwigger BSCP (Burp Suite Certified Practitioner) — heavily respected, hands-on web-only exam
- GWAPT (GIAC Web Application Penetration Tester)
- HTB CPTS (Certified Penetration Testing Specialist)
- OSWA (OffSec Web Assessor)
- eCPPT (eLearnSecurity Certified Professional Penetration Tester) — broader pentest, strong web component

### 18.4 Advanced / Expert-Level Web Application Security
- OSWE (OffSec Web Expert) — AWAE course, source-code-review-driven exploitation
- HTB CWEE (Certified Web Exploitation Expert)
- eWPTX (eLearnSecurity Web Application Penetration Tester eXtreme)
- GXPN (GIAC Exploit Researcher and Advanced Penetration Tester) — broader, advanced exploitation

### 18.5 Specialized / Regional Certifications
- CREST CRT (Registered Tester) — UK/EU recognized
- CREST CCT APP (Certified Web Application Tester) — advanced UK/EU web-specific
- OSCP (OffSec Certified Professional) — general pentest, widely required alongside web-specific certs

### 18.6 Suggested Certification Path
1. (Optional) Security+ or eJPT — build general footing
2. eWPT or CBBH — prove entry-level web testing skill
3. PortSwigger BSCP — the most respected pure hands-on web checkpoint
4. HTB CPTS or GWAPT — broaden into full pentest methodology
5. OSWE or HTB CWEE — expert-level, source-code-aware exploitation
