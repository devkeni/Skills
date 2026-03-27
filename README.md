<div align="center">

# 🧰 Skills Backup Library

<img src="https://readme-typing-svg.demolab.com?font=Inter&weight=700&size=26&duration=2600&pause=900&center=true&vCenter=true&width=900&lines=AI+agent+skills+backup+repo;OpenAI+%2B+community+skill+library;Provenance+tracked+and+public-safe+audited" alt="Typing SVG" />

<p>
  <img alt="repo purpose" src="https://img.shields.io/badge/purpose-backup%20%2F%20mirror-111827?style=for-the-badge">
  <img alt="public audit" src="https://img.shields.io/badge/public%20audit-passed-15803d?style=for-the-badge">
  <img alt="contains app code" src="https://img.shields.io/badge/app%20source%20code-not%20included-7f1d1d?style=for-the-badge">
</p>

<p>
  📦 Curated backup of AI coding-agent skills<br/>
  🔎 Best-effort provenance tracking<br/>
  🛡️ Checked before being exposed in a public repository
</p>

</div>

---

## ✨ What This Repo Is

This repository is a **backup/mirror of skills** used with coding agents such as Codex and similar tooling.

It exists to:

- keep a portable backup of the skill library
- preserve useful community and official skill bundles in one place
- make provenance and attribution easier to inspect
- avoid mixing TaskVoid application code with the skills collection

This repo is **not** an application source repository. It stores **skills only**.

---

## 🛡️ Public Safety Check

Before making this repo public, it was checked for:

- unrelated private project references
- personal infrastructure references
- real `.env` files, keys, tokens, SSH material, or certificates
- obvious hardcoded credentials
- scripts that looked like exfiltration or hidden credential harvesting

### Audit result

- No unrelated private project files were found in tracked content.
- No real secrets, private keys, `.env` files, or personal credentials were found in tracked content.
- No personal `Coolify`, `database`, `SMTP`, `SSH`, or app secrets were found in tracked content.
- Some folders intentionally contain **dummy credentials** or **bad examples** used by validator/testing skills. These are synthetic fixtures, not real secrets.
- The security/pentest skills remain in the repo because they are documentation/tooling content, not embedded access to any private system.
- Some skills intentionally document risky-but-explicit operational patterns such as `curl | bash`, webhook posting, or browser-cookie-based local extraction. They are not hidden exfiltration, but they should be reviewed before use.

If anything here still belongs to you and should not be public, open an issue or contact me and I will correct/remove it.

---

## 🧭 Provenance Policy

I did **not** want to publish this repo pretending authorship over work created by others.

So this README separates sources into:

- **Verified upstreams**: the original GitHub repo or creator is explicit in the bundle
- **Official catalog mirrors**: the skill matches the official Codex/OpenAI skill ecosystem
- **Best-effort local mirrors**: preserved here, but the original author/repo is not explicitly declared inside the bundled files

Where the original creator is not explicit, I prefer marking it honestly instead of inventing attribution.

---

## 🌍 Verified Upstreams

| Bundle | Included here | Verified creator / upstream | Link |
| --- | --- | --- | --- |
| Taste Skill family | `frontend-ui/taste-skill` and the related visual-style derivatives in `frontend-ui/` | Leonxlnx | [`github.com/Leonxlnx/taste-skill`](https://github.com/Leonxlnx/taste-skill) |
| AI Security Arsenal | `security/ai-security-arsenal` | Public upstream traced during audit | [`github.com/hardw00t/ai-security-arsenal`](https://github.com/hardw00t/ai-security-arsenal) |
| Spec-Kit workflow basis | `ai-apps/spec-kit-skill` | GitHub Spec-Kit toolkit | [`github.com/github/spec-kit`](https://github.com/github/spec-kit) |
| ChatGPT Apps examples basis | `ai-apps/chatgpt-apps` references official example workflow | OpenAI Apps SDK examples | [`github.com/openai/openai-apps-sdk-examples`](https://github.com/openai/openai-apps-sdk-examples) |
| Autonomous Codex helper basis | `ai-apps/autonomous-skill` references Codex CLI directly | OpenAI Codex | [`github.com/openai/codex`](https://github.com/openai/codex) |

### Notes

- `Taste Skill` explicitly references its official site and GitHub repo inside the bundled README.
- `AI Security Arsenal` is preserved as a public upstream mirror traced during audit. If a more canonical upstream should be credited, I will update this README.
- `spec-kit-skill` is a skill wrapper around the GitHub `spec-kit` workflow/tooling. That link is the concrete upstream dependency it declares.

---

## 🤖 Official Catalog Mirrors

Several folders in this repo mirror or closely track skills that are also part of the **official Codex/OpenAI skill ecosystem**.

Primary public references:

- [`github.com/openai/skills`](https://github.com/openai/skills)
- [`github.com/openai/codex`](https://github.com/openai/codex)

Examples in this repo that align with the official catalog include:

- `backend-devops/aspnet-core`
- `data-documents/doc`
- `data-documents/jupyter-notebook`
- `data-documents/pdf`
- `data-documents/spreadsheet`
- `github-devtools/gh-address-comments`
- `github-devtools/gh-fix-ci`
- `github-devtools/yeet`
- `media-creative/imagegen`
- `media-creative/slides`
- `media-creative/sora`
- `media-creative/speech`
- `media-creative/transcribe`
- `security/security-best-practices`
- `security/security-ownership-map`
- `security/security-threat-model`
- `testing-automation/playwright`
- `testing-automation/playwright-interactive`
- `testing-automation/screenshot`

Some frontend and deployment skills here also match the same ecosystem closely, even when the exact original public repo is not stated inside the local bundle.

---

## 🧪 Best-Effort Local Mirrors

These folders are preserved here because they are useful, but the exact original author/repo is **not explicitly declared inside the local files**:

- `ai-apps/claude-skill`
- `ai-apps/deep-research`
- `ai-apps/kiro-skill`
- a large part of `backend-devops/`
- part of `frontend-ui/`
- part of `media-creative/`
- part of `notion-productivity/`

That does **not** mean they are unsafe.

It means only this:

- the bundle is present locally
- the content was preserved
- the exact creator attribution still needs stronger provenance if I want per-skill authorship precision

If you are the original author of any mirrored skill here and want:

- stronger credit
- a corrected upstream link
- removal from this backup repo

open an issue and I will update it.

---

## 🗂️ Repo Layout

```text
ai-apps/
backend-devops/
data-documents/
frontend-ui/
github-devtools/
media-creative/
notion-productivity/
security/
testing-automation/
```

### Folder guide

- `ai-apps/` — agent workflows, app SDK, research, autonomous/spec-driven helpers
- `backend-devops/` — infra, CI/CD, Docker, Terraform, Cloudflare, Kubernetes, validators
- `data-documents/` — docx, pdf, notebooks, spreadsheets
- `frontend-ui/` — Figma, frontend implementation, design systems, visual taste packs
- `github-devtools/` — PR review, CI triage, PR publishing workflows
- `media-creative/` — images, slides, video, speech, transcription
- `notion-productivity/` — Notion capture, research, planning, execution workflows
- `security/` — secure coding and AppSec / pentest skill bundles
- `testing-automation/` — Playwright, screenshots, browser automation

---

## ⚠️ Security / Pentest Content Notice

This repo contains security-oriented skills such as:

- threat modeling
- secure coding
- SAST/SCA orchestration
- DAST and pentest workflow guidance
- mobile and cloud security assessment skills

These are kept here for **authorized security work, education, review, and testing**.

Nothing in this backup repo grants access to private systems. The repo contains skills and documentation, not live credentials.

---

## 🙌 Credit & Respect

Big thanks to the original creators, maintainers, and communities behind these skills and the broader agent-tooling ecosystem.

This repository is intended as:

- a backup
- a working mirror
- a provenance-aware archive

It is **not** intended to erase original authorship.

---

## 📬 Attribution Fixes

If any attribution here is incomplete or incorrect, please open an issue or pull request with:

- the correct upstream repo
- the correct creator/organization name
- the folder(s) affected

I will update the README accordingly.
