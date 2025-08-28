# 🛡️ Code of Ethics — Cybersecurity Portfolio

**Author:** JW Britz  
**Effective Date:** 2025-08-28  
**Applies to:** All activities, artifacts, and workflows within this repository.

---

## 1. Purpose

This Code of Ethics defines the boundaries, responsibilities, and standards governing all cybersecurity work represented in this portfolio. It exists to:
- Safeguard the rights, privacy, and property of individuals and organizations.
- Ensure **lawful, authorized** security testing.
- Maintain **integrity, professionalism, and operational discipline**.

---

## 2. Ethical Foundations

| Principle | Commitment |
|-----------|------------|
| **Legality** | Every test, scan, or simulation is conducted on systems I own, have explicit written permission to test, or are intentionally provided for public training (e.g., TryHackMe, OverTheWire). |
| **Authorization** | No activity occurs without prior approval from the rightful owner; scope and boundaries are defined in writing before engagement. |
| **Integrity** | Results are never falsified. Evidence is stored with verifiable hashes to prevent tampering. |
| **Confidentiality** | Sensitive information encountered during testing is safeguarded and never disclosed without consent. |
| **Non‑Maleficence** | No action is taken that could harm systems, data, reputation, or people, beyond agreed‑upon and mitigated test parameters. |
| **Transparency** | Reports clearly differentiate between observed facts, inferred conclusions, and recommendations. |

---

## 3. Operational Conduct

1. **Lawful Scope Only** — Activities stay within permitted ranges defined by:
   - Legal jurisdictions
   - Written contracts or agreements
   - Training platform Terms of Service

2. **Controlled Impact** — All exploitation is contained within isolated lab or authorized environments.  
   - No pivoting to non‑scoped networks  
   - No data exfiltration beyond what is essential for proof

3. **Evidence Hygiene** — Every log, packet capture, and screenshot is:
   - Sanitized to remove personal identifiers, secrets, or sensitive IP addresses
   - Timestamped and hashed (SHA‑256) for chain‑of‑custody integrity

4. **Disclosure Protocol** — Any real‑world vulnerability discovery triggers:
   - Immediate notification to the asset owner or responsible security contact
   - No public disclosure until mitigation is verified and approved

5. **Tool Discipline** — Use of automated tools is governed by:
   - Understanding of how the tool works and potential side effects
   - Respect for rate limits and resource consumption
   - Documentation of tool version and configuration in `environment.json`

---

## 4. Professional Standards

- **Documentation Excellence** — Every deliverable, from lab write‑up to project report, meets the dual standard of technical accuracy and executive readability.
- **Continuous Learning** — Skills, techniques, and tools are kept current with industry best practices and evolving threat landscapes.
- **Peer Accountability** — I welcome constructive critique from trusted peers, mentors, or industry leaders to improve my craft.
- **Reputation First** — I operate under the principle that my professional reputation is worth more than any shortcut, exploit, or unauthorized advantage.

---

## 5. Compliance & Enforcement

- This code applies to all commits, branches, artifacts, and external communications referencing this repository.
- Breach of these principles:
  - Triggers immediate remediation and documentation of the corrective actions.
  - May result in removal of offending content and disclosure of the violation in the repo changelog for transparency.

---

## 6. Statement of Honor

> *“My skills are my responsibility. I will use them to protect, not to harm; to strengthen, not to exploit.  
> Every artifact here is a testament to discipline, integrity, and respect for the craft of cybersecurity.”*

---

> I am accountable for these standards and the impact of my work.

**Signed:**  
`J.W. BRITZ`  
