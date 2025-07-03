# 🛡️ Browser Extension Audit & Hardening Task

## 🔍 Objective

The primary objective of this task was to conduct a meticulous security audit of browser extensions installed in Google Chrome. This entailed analyzing each extension's privileges, provenance, and operational necessity. The goal was to identify superfluous, risky, or inactive components and eliminate them to minimize the browser's attack surface and optimize digital hygiene.

---

## 🧩 Extension Evaluation Summary

| Extension Name                     | Status    | Action Taken | Justification Summary                                      |
|-----------------------------------|-----------|--------------|-------------------------------------------------------------|
| AdBlock for YouTube™              | On        | ❌ Removed   | Excessive permissions and unnecessary site-wide access     |
| AliPrice for Flipkart             | Off       | ❌ Removed   | Medium-risk tracker, unused, limited to Flipkart           |
| Memefy This                       | Off       | ❌ Removed   | Suspicious due to full-site access for meme functionality  |
| Picture-in-Picture (by Google)    | On        | ✅ Kept      | Trusted source, justified utility, non-intrusive           |
| NeoExamShield                     | Off       | ❌ Removed   | Elevated control over browser, exam-only utility           |
| Loom Screen Recorder              | Off       | ❌ Removed   | High-risk screen capture with wide permissions             |
| Google Docs Offline               | Off       | ✅ Kept      | Official, limited scope, supports offline productivity     |

---

## 📋 Detailed Extension Analyses

### 1️⃣ AdBlock for YouTube™
- **Permissions:** Full data access on all websites, read browsing history  
- **Risk Level:** ⚠️ Elevated  
- **Action:** ❌ *Removed*  
- **Additional Notes:**
  - Capable of intercepting and modifying HTTP requests for ad removal, which could be exploited for tracking or injection.  
  - Many ad blockers have been caught in the past reselling anonymized data or injecting their own ads, raising trust concerns.

---

### 2️⃣ AliPrice Shopping Assistant for Flipkart
- **Permissions:** Flipkart & AliPrice domain access  
- **Risk Level:** ⚠️ Medium  
- **Action:** ❌ *Removed*  
- **Additional Notes:**
  - Known for affiliate redirection and price behavior monitoring which may violate user consent norms.  
  - Operates silently in the background and can passively log e-commerce behavior patterns for marketing purposes.

---

### 3️⃣ Memefy This
- **Permissions:** Access to all websites  
- **Risk Level:** 🔴 High  
- **Action:** ❌ *Removed*  
- **Additional Notes:**
  - Functionality does not justify the extreme breadth of permissions granted.  
  - May present a facade of utility while acting as a vehicle for client-side JavaScript injection or persistent tracking.

---

### 4️⃣ Picture-in-Picture (by Google)
- **Permissions:** Full-site access  
- **Risk Level:** ✅ Low  
- **Action:** ✅ *Kept*  
- **Additional Notes:**
  - Developed and maintained by Google, ensuring frequent security updates and patch compliance.  
  - Enhances productivity and multitasking without maintaining background processes or unauthorized access.

---

### 5️⃣ NeoExamShield
- **Permissions:** App and extension management, browsing history, content control  
- **Risk Level:** 🔴 Critical  
- **Action:** ❌ *Removed*  
- **Additional Notes:**
  - Grants administrative control over the Chrome environment, which could be leveraged to disable other security tools.  
  - Designed for exam environments only; leaving it installed outside assessment windows introduces unnecessary surveillance potential.

---

### 6️⃣ Loom – Screen Recorder & Capture
- **Permissions:** All-site access, screen capture rights  
- **Risk Level:** ⚠️ Elevated  
- **Action:** ❌ *Removed*  
- **Additional Notes:**
  - Capable of capturing browser visuals, microphone input, and even webcam feeds—an expansive privacy vector.  
  - Inactive extensions with such capabilities pose latent threats if re-enabled maliciously or via third-party triggers.

---

### 7️⃣ Google Docs Offline
- **Permissions:** Restricted to Google Docs and Drive  
- **Risk Level:** ✅ Minimal  
- **Action:** ✅ *Kept*  
- **Additional Notes:**
  - Limited scope and sandboxed environment ensures low security exposure.  
  - Useful for continuity in low-connectivity scenarios; no background network communication when disabled.

---

## ✅ Conclusion

This comprehensive audit enhanced the security posture of the browser environment by eliminating dormant, extraneous, and privilege-heavy extensions. Adherence to the principle of **least privilege** and awareness of **extension provenance** are vital in curating a secure, efficient digital workspace. Proactive extension management remains a cornerstone of browser-side cybersecurity defense.


