# pv-cra-console
A six-module PV/CRA portfolio prototype — case coding, duplicate detection, query generation, literature triage, and risk-based site monitoring, built on ICH E2A, WHO-UMC, and ICH E6(R2) principles.
# PV / CRA Console — Static Demo

A six-module portfolio prototype covering pharmacovigilance and clinical research
associate workflows: case coding, duplicate detection, follow-up query generation,
literature triage, site risk scoring (RBQM), and an aggregate dashboard.

This is a **static demo build** — modules 1 to 4 show pre-computed outputs for
preset example cases (no live API call, no key required), so it is safe to host
publicly and will never break or incur any cost. Modules 5 and 6 are fully live,
rule-based JavaScript with no external dependency.

**Live demo:** replace this line with your GitHub Pages URL once deployed, e.g.
`https://<your-username>.github.io/pv-cra-console/`

## How to host this for free on GitHub Pages

1. Create a new **public** repository on GitHub (e.g. `pv-cra-console`).
2. Upload `index.html` (and this `README.md`) to the root of the repository.
   - Easiest way: on the repo page, click **Add file → Upload files**, drag in
     `index.html`, and commit.
3. Go to the repo's **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, select `main` and folder `/ (root)`, then click **Save**.
6. Wait about a minute, then refresh the Pages settings page — it will show a
   live URL in the form `https://<your-username>.github.io/pv-cra-console/`.
7. That URL is your permanent, free, public link — put it on LinkedIn, your CV,
   or your Sharma MedInsights page.

No build step, no server, no API key — it's a single HTML file.

## Notes for viewers / reviewers

- This tool does not use the licensed MedDRA® dictionary. Preferred Term / SOC /
  HLGT / HLT terms are illustrative approximations for educational purposes.
- Seriousness logic follows ICH E2A criteria; causality logic follows the
  WHO-UMC causality categories.
- Site risk scoring (Module 5) uses a transparent, fixed weighted formula
  consistent with ICH E6(R2) risk-based quality management principles.
- Built as a personal portfolio project by Sunny (Sharma MedInsights).
