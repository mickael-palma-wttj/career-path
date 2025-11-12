# Security

**Criterion:** Understanding security principles, building secure systems, threat awareness, and compliance responsibility.

Security is everyone's responsibility, not just a specialist role. Every engineer who writes code that handles data makes security decisions daily. The best security is built in from the start, not added after.

---

## 📋 Quick Summary

| Level | Expectation | Impact |
|-------|-------------|--------|
| **Developing (0.0-1.0)** | Learning security basics; security not top of mind | Vulnerabilities in code; security debt |
| **Competent (1.0-2.0)** | Follows security practices; thinks about common issues | Avoids obvious vulnerabilities |
| **Proficient (2.0-3.0)** | Builds secure systems; proactively identifies risks | Systems designed with security in mind |
| **Expert (3.0-3.5)** | Security expert; mentors on threat modeling | Security decisions are sound; mentors others |
| **Authority (3.5-4.0)** | Org security authority; shapes security culture | Org security posture improved; compliance met |

---

## 🎯 Definition

**Security** encompasses five interconnected capabilities:

### 1. **Secure Coding**
Writing code without common vulnerabilities. Understanding OWASP top 10. Building code that resists attacks. Making security-conscious choices in implementation.

### 2. **Threat Awareness**
Understanding attack vectors. Thinking like an attacker. Knowing common threats in your domain. Anticipating how systems could be compromised.

### 3. **Risk Thinking**
Understanding security implications of design decisions. Evaluating risk/benefit trade-offs. Knowing what risks are acceptable vs. unacceptable. Making risk-conscious choices.

### 4. **Compliance & Regulation**
Understanding relevant compliance requirements (SOC 2, HIPAA, GDPR, etc.). Meeting regulatory requirements. Understanding audit requirements. Building systems that can be audited.

### 5. **Security Advocacy**
Promoting security mindset across engineering. Helping others understand security. Pushing for security investments. Building security culture.

---

## 📊 Detailed Level Descriptions

### 🟦 Developing (0.0 - 1.0)

**Core Behaviors:**
- Security not top of mind
- Doesn't know OWASP top 10
- Treats security as external concern
- Implements security when told
- Limited threat awareness
- Compliance is checkbox item

**What You'd See:**
- "Is this secure?" asked after code written
- Security feedback taken as criticism
- Not thinking about attack vectors
- Doesn't ask security questions
- Follows security checklist without understanding

**What Success Looks Like:**
- Learn security fundamentals
- Understand common vulnerabilities
- Start thinking about threats
- Ask security questions
- Understand why security matters

**Development Focus:**
- Learn OWASP top 10
- Understand common vulnerabilities
- Build threat awareness
- Develop security mindset
- Ask security questions

---

### 🟩 Competent (1.0 - 2.0)

**Core Behaviors:**
- Follows security practices and checklists
- Avoids obvious vulnerabilities (SQL injection, XSS, etc.)
- Asks for security review before shipping
- Aware security matters but not proactive
- Learning threat modeling
- Starting to think about compliance

**What You'd See:**
- Code follows security checklist
- No obvious vulnerabilities present
- Security reviewed and approved
- Asks "is this secure?" questions
- Shows awareness of security concerns
- Needs guidance on security decisions

**Specific Examples:**
- "I used parameterized queries like you showed me"
- "I got a security review before shipping"
- "What's the right way to store this sensitive data?"

**What Success Looks Like:**
- No vulnerabilities in code
- Security-conscious decisions
- Good threat awareness emerging
- Questions security assumptions
- Learns from security reviews

**Development Focus:**
- Understand threat models
- Proactive security thinking
- Deeper vulnerability knowledge
- Build security instincts
- Learn compliance requirements

---

### 🟧 Proficient (2.0 - 3.0)

**Core Behaviors:**
- Builds security in from design phase
- Proactively identifies security risks
- Thinks through threat models
- Code exemplifies secure practices
- Helps others write secure code
- Compliance-minded in design
- Security considerations visible

**What You'd See:**
- Security considered in design discussions
- No security issues found in code reviews
- Proactively identifies risks
- Threat model documented
- Helps others understand security
- Code examples used for training
- Compliance requirements incorporated

**Specific Examples:**
- "Before we design this, I want to threat model it. Here are attack vectors I'm thinking about..."
- "This feature needs encryption. Here's why and how I'd implement it"
- "For GDPR compliance, we need to handle data this way..."
- Code review comment: "This could be vulnerable to timing attacks; here's a fix"

**Evidence:**
- No security issues in their code
- Security considered proactively
- Others ask them for security input
- Threat models created and explained
- Helps team improve security

**What Success Looks Like:**
- Recognized for security expertise
- Helping team improve security practices
- Security initiatives from them
- Mentoring others on security

**Development Focus:**
- Mentor others on security
- Lead security improvements
- Improve org's security practices
- Think strategically about security
- Move toward security leadership

---

### 🟨 Expert (3.0 - 3.5)

**Core Behaviors:**
- Exceptionally security-aware
- Threat modeling is natural
- Identifies novel security risks
- Mentors others on security practices
- Security decisions are sound
- Goes beyond compliance
- Proactively improves security

**What You'd See:**
- Sought for security consultation
- Identifies sophisticated attack vectors
- Mentors team on threat modeling
- Identifies security issues others miss
- Proactively improves security
- Pushes org beyond minimum compliance
- Creates security patterns

**Specific Examples:**
- "I identified a potential timing attack in our auth code"
- Mentored team on cryptographic practices
- "Here's how we should think about data classification"
- "Our supply chain dependencies have these security risks..."

**Evidence:**
- Recognized as security expert
- Asked for security consultation
- Mentors on security practices
- Identifies subtle vulnerabilities
- Drives security improvements
- Org security posture improves

**What Success Looks Like:**
- Set security standards for team
- Multiple people mentored on security
- Security improvements from their leadership
- Org security culture influenced by them

**Development Focus:**
- Scale security impact across organization
- Lead security initiatives
- Mentor more people
- Shape org security culture
- Could move to security/leadership

---

### 🟥 Authority (3.5 - 4.0+)

**Core Behaviors:**
- Org's security authority
- Sets security standards
- Shapes org security culture
- Influences org-wide security decisions
- Others follow their security practices
- Compliance decisions from them
- Org security improved

**What You'd See:**
- Org security standards from them
- Others model their security practices
- Org security posture improved
- Security reviews reference their standards
- Compliance met due to their guidance
- Security culture influenced by them
- Fewer vulnerabilities org-wide

**Specific Examples:**
- "This is how we approach security at our organization"
- Org adopted their security review process
- Compliance improved based on their initiatives
- "New engineers learn security from these practices"

**Evidence:**
- Org recognizes as security authority
- Org security standards from them
- Compliance met consistently
- Fewer vulnerabilities org-wide
- Security culture changed
- Multiple teams influenced

---

## 📊 Common Vulnerabilities & Mitigations

### OWASP Top 10 Framework

| Vulnerability | Risk | Mitigation |
|---|---|---|
| SQL Injection | Very High | Use parameterized queries, ORM, input validation |
| Authentication Bypass | Very High | Strong auth, MFA, proper session management |
| Sensitive Data Exposure | High | Encryption, PII handling, key management |
| XML External Entity | Medium | Disable DTD, use safe XML parsers |
| Access Control | High | Proper authorization checks, RBAC |
| Security Misconfiguration | Medium | Security hardening, dependency updates |
| Cross-Site Scripting (XSS) | High | Input validation, output encoding, CSP |
| Insecure Deserialization | Medium | Avoid untrusted deserialization |
| Using Components with Known Vulns | Medium | Dependency scanning, keep updated |
| Insufficient Logging & Monitoring | Medium | Audit logs, alerts, monitoring |

---

## ❓ Assessment Questions

**For Developing → Competent:**
- What are the top OWASP vulnerabilities?
- How would someone attack this feature?
- Where should we be careful about user input?
- Why is parameterized queries important?

**For Proficient → Expert:**
- What security risks do you see in this design?
- Walk me through your threat model for this feature.
- How would you model attacks on this system?
- What are the compliance implications here?

**For Expert → Authority:**
- How should we approach security organization-wide?
- What security investments would have biggest impact?
- How do we build security culture across engineering?
- What's our threat model for [critical system]?

---

## 👀 Evidence to Look For

### At Proficient Level (2.0-3.0)
- ✅ Security considered in design
- ✅ No security issues found in their code
- ✅ Proactively identifies risks
- ✅ Follows compliance requirements
- ✅ Helps others understand security
- ✅ Threat models created

### At Expert Level (3.0-3.5)
- ✅ Sought for security consultation
- ✅ Teaches others about threat modeling
- ✅ Stays current on security topics
- ✅ Identifies subtle vulnerabilities
- ✅ Drives security improvements
- ✅ Org security improves

### At Authority Level (3.5-4.0)
- ✅ Org follows their security practices
- ✅ Security culture improved
- ✅ Fewer vulnerabilities in shipped code
- ✅ Compliance met consistently
- ✅ Others model their approach
- ✅ Security standards adopted org-wide

### Negative Indicators (Any Level)
- ❌ Security issues in code
- ❌ No threat awareness
- ❌ Defensive about security feedback
- ❌ Skipping security reviews
- ❌ Not thinking about compliance
- ❌ Treating security as afterthought
- ❌ No encryption of sensitive data
- ❌ Can't explain security decisions
- ❌ Ignoring security warnings
- ❌ No audit logging

---

## 🔗 Related Skills & Competencies

**Directly Connected:**
- **Technical Understanding** (Engineering Craft) - Deep tech knowledge reveals security implications
- **Software Architecture** (Engineering Craft) - Secure systems are designed securely
- **Writing Code** (Engineering Craft) - Secure code is foundational
- **Communication** (Soft Skills) - Advocating for security practices

**Indirectly Connected:**
- **Initiative** (Soft Skills) - Proactively improving security
- **Business Acumen** (Soft Skills) - Understanding compliance and risk
- **Objectivity** (Soft Skills) - Evaluating security risks rationally
- **Team Leadership** (Leadership) - Building security culture

---

## � Development Goals & Progression Paths

### Competent → Proficient
**Goal:** "Build security in from design; mentor others"

**Specific Actions:**
- [ ] Threat model [new feature]; document attack vectors
- [ ] Review [existing system] for security issues
- [ ] Learn [compliance framework] relevant to our business
- [ ] Create security guide for [feature type]
- [ ] Mentor one person on threat modeling
- [ ] Design [new feature] with security from start
- [ ] No security issues in code review

**Timeline:** 6-12 months

---

### Proficient → Expert
**Goal:** "Identify novel risks; mentor widely; improve org security"

**Specific Actions:**
- [ ] Mentor 2+ people on security practices
- [ ] Conduct security assessment of [critical system]
- [ ] Identify and document security risks org-wide
- [ ] Create security patterns adopted by team
- [ ] Stay current: conferences, articles, training
- [ ] Teach security workshop or write guide
- [ ] Find and help fix subtle vulnerabilities

**Timeline:** 12-24 months

---

### Expert → Authority
**Goal:** "Shape org's security approach; scale impact"

**Specific Actions:**
- [ ] Define org's security standards and practices
- [ ] Lead security improvement initiative
- [ ] Mentor leaders on security thinking
- [ ] Build security review process org-wide
- [ ] Create security guidelines adopted org-wide
- [ ] Measure and improve org security
- [ ] External visibility: conference or article on security

**Timeline:** 2-3+ years

---

## � Detailed Development Guidance

### Learning Threat Modeling

**Threat Modeling Framework (STRIDE):**

- **Spoofing**: Can someone pretend to be someone else?
- **Tampering**: Can someone modify data or systems?
- **Repudiation**: Can someone deny their actions?
- **Information Disclosure**: Can someone access sensitive data?
- **Denial of Service**: Can someone prevent legitimate use?
- **Elevation of Privilege**: Can someone get higher access?

**How to Threat Model:**
1. **Understand the system** - Components, data flow
2. **Identify assets** - What needs protection?
3. **List threats** - What could go wrong? (Use STRIDE)
4. **Rate risks** - Likelihood × Impact
5. **Plan mitigations** - How do we prevent/detect/respond?

### Building Security Practices

**Secure Coding Checklist:**

- [ ] **Input Validation**: Validate all user input
- [ ] **Output Encoding**: Encode output appropriately
- [ ] **Authentication**: Strong, multi-factor where sensitive
- [ ] **Authorization**: Check permissions explicitly
- [ ] **Encryption**: Encrypt sensitive data at rest and in transit
- [ ] **Error Handling**: Don't leak sensitive info in errors
- [ ] **Logging**: Log security events for auditing
- [ ] **Dependency Management**: Keep dependencies updated
- [ ] **Secrets Management**: Never hardcode secrets
- [ ] **API Security**: API keys, rate limiting, CORS

### Compliance & Regulation

**Common Compliance Frameworks:**

| Framework | Purpose | Key Focuses |
|---|---|---|
| SOC 2 | Demonstrate security, availability, integrity | Access controls, monitoring, incident response |
| HIPAA | Healthcare data privacy | Encryption, access controls, audit logs |
| GDPR | Data privacy (EU) | Data protection, user rights, breach notification |
| PCI-DSS | Payment card data | Encryption, access controls, monitoring |
| ISO 27001 | General information security | Policies, procedures, controls |

**Understanding Your Compliance Requirements:**
1. Know what regulations apply to your business
2. Understand what data needs protection
3. Learn the requirements
4. Design systems to meet them
5. Build audit capability

---

## 💡 Key Principles

### 1. **Security is Everyone's Responsibility**
Security isn't a specialist role. Every engineer who handles data makes security decisions. Build security culture where all engineers own it.

### 2. **The Best Security is Built In**
Building security into design is far cheaper than bolting it on. Design systems securely from the start.

### 3. **Threat Modeling Prevents Problems**
Thinking like an attacker before deployment catches issues that testing won't. Make threat modeling routine.

### 4. **Defense in Depth**
No single security control is perfect. Layer multiple controls. If one fails, others catch it.

### 5. **Security Must Balance Usability**
Security that's too hard to use gets bypassed. Find balance between security and usability.

### 6. **Compliance is Minimum, Not Maximum**
Meeting compliance requirements is minimum bar. Security should exceed compliance. Build better than required.

---

## 🎯 Red Flags & Warnings

- ⚠️ **Security issues in code review** — Not reviewing for security
- ⚠️ **No threat models** — Not thinking about threats proactively
- ⚠️ **Sensitive data unencrypted** — Critical vulnerability
- ⚠️ **No authentication/authorization** — Open to attacks
- ⚠️ **Hardcoded secrets** — Credentials exposed
- ⚠️ **No audit logging** — Can't detect breaches
- ⚠️ **Dependencies out of date** — Known vulnerabilities present
- ⚠️ **Compliance ignored** — Regulatory risk
- ⚠️ **No security reviews** — Vulnerabilities missed
- ⚠️ **Security treated as afterthought** — Culture problem

---

**Remember:** Security is everyone's responsibility. The best security is built in from the start, not added after.
