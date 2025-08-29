# Badge Placement Map & Syntax

**Single source of visual authority** for the Executive Cybersecurity Portfolio.  
All placements below reference the **sole master asset**:

```
.\branding\executive-badge.svg.png
```

---

## Asset Policy

- **File:** `executive-badge.svg.png`
- **Master location:** `.\branding\`
- **No duplicates** — all references point to this single file with correct relative paths.
- **PNG** ensures consistent rendering in GitHub, PDFs, and exports.
- **SVG layer preserved** inside PNG for design fidelity.

---

## Global Placement Rules

- **Consistency = Authority** — same file, controlled widths, disciplined alignment per document type.
- **No CSS reliance** — use `align` and `width` attributes only (GitHub strips most inline CSS).
- **Always before H1** — crest precedes the document title in all branded files.
- **Alt text = Identity** — format: `"JW Britz — [Document Context]"`.
- **No data pollution** — never embed in raw data, evidence, or config files.

---

## Placement Map

| Document | Alignment | Width (px) | Link wrap | Purpose |
|---|---|---:|---|---|
| `/README.md` | Center | 420 | Yes | Hero identity — portfolio entry point |
| `/GOVERNANCE.md` | Left | 110 | Optional | Sealed governance charter |
| `/SECURITY.md` | Center | 160 | Optional | Policy banner |
| `/CONTRIBUTING.md` | Right | 140 | Optional | Operational charter |
| `/CHANGELOG.md` | Right | 120 | No | Discreet change log seal |
| `/branding/README.md` | Center | 160 | Optional | Brand guidelines index |
| `/labs/README.md` | Center | 140 | Optional | Lab index letterhead |
| `/incident-response/README.md` | Center | 140 | Optional | Incident playbook banner |
| `/executive-summaries/README.md` | Left | 120 | Optional | Letterhead |
| `/evidence/README.md` | Center | 120 | No | Watermark‑style presence |
| `/ci-cd/README.md` | Right | 120 | No | Discreet technical seal |

---

## Paste‑Ready Snippets

**Root README hero:**
```markdown
<p align="center">
  <a href="./README.md">
    <img src="./branding/executive-badge.svg.png" alt="JW Britz — Executive Cybersecurity Portfolio" width="420">
  </a>
</p>
```

**Governance (sealed, top‑left):**
```markdown
<img align="left" src="./branding/executive-badge.svg.png" alt="JW Britz — Governance Charter" width="110">
```

**Security Policy banner:**
```markdown
<p align="center">
  <img src="./branding/executive-badge.svg.png" alt="JW Britz — Security Policy" width="160">
</p>
```

**Contributing (right stamp):**
```markdown
<p align="right">
  <img src="./branding/executive-badge.svg.png" alt="JW Britz — Operational Charter" width="140">
</p>
```

**Changelog (small stamp):**
```markdown
<p align="right">
  <img src="./branding/executive-badge.svg.png" alt="JW Britz — Changelog" width="120">
</p>
```

**Nested section example (labs):**
```markdown
<p align="center">
  <img src="../branding/executive-badge.svg.png" alt="JW Britz — Labs" width="140">
</p>
```

> Adjust relative paths (`../` or `../../`) for depth.

---

## Update Protocol

- **Single‑file discipline** — all docs point to the master file in `.\branding\`.
- **Version control** — when updated, rename (e.g., `executive-badge.v2.svg.png`) and update all refs in one commit.
- **Double‑check in GitHub view** for actual rendering.
- **Paired commits** — always update this `badge-placement.md` and `CHANGELOG.md` together for traceability.

---

## Pre‑Push Checklist

- ✅ Correct path + filename.
- ✅ Approved width for doc type.
- ✅ Alt text includes name + context.
- ✅ Alignment matches table.
- ✅ No drift into unapproved folders.

---

## Appendix A — ASCII Badge Placement Field Diagram

```
                  ┌───────────────────────────┐
                  │       /README.md          │
                  │  [CENTER | 420px | LINK]  │
                  └────────────┬──────────────┘
                               │
    ┌──────────────────────────┼───────────────────────────┐
    │                          │                           │
┌───▼───┐                 ┌────▼────┐                 ┌────▼────┐
│GOVERN.│                 │SECURITY │                 │CONTRIB. │
│LEFT110│                 │CENT160  │                 │RIGHT140 │
└───┬───┘                 └────┬────┘                 └────┬────┘
    │                          │                           │
    │                ┌─────────▼──────────┐                │
    │                │   CHANGELOG        │                │
    │                │  RIGHT | 120px     │                │
    │                └────────┬───────────┘                │
    │                         ...                          │
    ▼                                                      ▼
 BRANDING                                             CI/CD Section
 CENTER 160px                                         RIGHT 120px
    │
    ▼
  LABS
 CENTER 140px
    │
    ▼
 INCIDENT RESPONSE
 CENTER 140px
    │
    ▼
 EXECUTIVE SUMMARIES
 LEFT 120px
    │
    ▼
 EVIDENCE
 CENTER 120px
```

**Legend:**
- **CENTER / LEFT / RIGHT** = alignment
- **[px]** = badge width
- **LINK** = wrapped in anchor to root README
- All nodes reference: `.\branding\executive-badge.svg.png`

---

**Command presence in pixels.** One badge, one standard — deployed with precision.

