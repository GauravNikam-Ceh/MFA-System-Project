# 🔐 Multi-Factor Authentication (MFA) System

> A research and implementation project focused on studying and evaluating enterprise-grade Multi-Factor Authentication mechanisms to strengthen identity verification and access control.

---

## 📌 Project Overview

This project explores how Multi-Factor Authentication (MFA) works across different methods and enterprise environments. The goal was to understand, compare, and document various authentication mechanisms and their security strengths and weaknesses.

MFA adds an extra layer of security by requiring users to verify their identity through **two or more factors**:
- 📱 Something you **have** (OTP, Authenticator App)
- 🔑 Something you **know** (Password)
- 👁️ Something you **are** (Biometrics)

---

## 🎯 Objectives

- Study and compare different MFA methods used in real-world enterprise environments
- Understand the security benefits and limitations of each method
- Document best practices for MFA implementation in organizations
- Analyze common MFA bypass attacks and how to prevent them

---

## 🛠️ Tools & Technologies Used

| Tool/Technology | Purpose |
|----------------|---------|
| Google Authenticator | TOTP-based OTP testing |
| Microsoft Authenticator | Enterprise MFA simulation |
| Kali Linux | Security testing environment |
| Burp Suite | Analyzing authentication requests |
| Python | Simulating OTP generation (TOTP/HOTP) |

---

## 🔬 MFA Methods Studied

### 1. SMS-Based OTP
- One-Time Password sent via SMS to registered mobile number
- ✅ Easy to implement
- ⚠️ Vulnerable to SIM swapping and SS7 attacks

### 2. Authenticator Apps (TOTP)
- Time-based One-Time Passwords generated every 30 seconds
- Apps: Google Authenticator, Microsoft Authenticator
- ✅ More secure than SMS
- ✅ Works offline

### 3. Biometric Authentication
- Fingerprint, Face Recognition, Retina Scan
- ✅ Highly secure and user-friendly
- ⚠️ Privacy concerns and spoofing risks

### 4. Hardware Tokens
- Physical devices generating OTPs (e.g. RSA SecurID)
- ✅ Very secure
- ⚠️ Expensive and easy to lose

---

## 🔬 Methodology

### Step 1: Research & Comparison
- Studied each MFA method in depth
- Compared security levels, usability, and implementation cost

### Step 2: Simulation & Testing
- Simulated OTP generation using Python (TOTP algorithm)
- Tested authentication flows using Burp Suite to intercept requests
- Analyzed how MFA tokens are validated server-side

### Step 3: Attack Analysis
- Studied common MFA bypass techniques:
  - OTP phishing
  - SIM swapping
  - Real-time phishing proxies (e.g. Evilginx2)
- Documented mitigation strategies for each attack

### Step 4: Best Practice Documentation
- Created enterprise MFA implementation guidelines

---

## 📊 MFA Methods Comparison

| Method | Security Level | User Friendly | Cost | Recommended |
|--------|---------------|---------------|------|-------------|
| SMS OTP | Medium | ✅ High | Low | ⚠️ Avoid for sensitive systems |
| Authenticator App | High | ✅ High | Free | ✅ Yes |
| Biometrics | Very High | ✅ Very High | Medium | ✅ Yes |
| Hardware Token | Very High | Medium | High | ✅ For critical systems |

---

## 📚 Key Learnings

- SMS OTP is the weakest MFA method due to SIM swap vulnerabilities
- TOTP-based authenticator apps provide the best balance of security and usability
- MFA significantly reduces the risk of credential-based attacks
- Even MFA can be bypassed — defense in depth is essential

---

## 🏆 Certifications Supporting This Work

- Certified Ethical Hacker (CEH v12) – EC-Council
- Cyber Security & Ethical Hacking Internship – Spinnaker Analytics (via BIA)

---

## 👤 Author

**Gaurav Rakesh Nikam**  
PG Diploma in Cyber Security & Ethical Hacking – Boston Institute of Analytics, Mumbai  
📧 gauravrakeshnikam@gmail.com  
📍 Pune, Maharashtra

---

> ⚠️ **Disclaimer:** This project was conducted in a controlled lab environment for educational purposes only. All testing was performed on intentionally vulnerable or simulated applications. No real systems were targeted.
