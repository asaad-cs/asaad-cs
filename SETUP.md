# Setup Guide — GitHub Profile README

## What This Is

A GitHub Profile README lives in a special repository named exactly the same as your GitHub username.
For example, if your GitHub handle is `ahmed-alfaidi`, the repo must be `ahmed-alfaidi/ahmed-alfaidi`.

---

## Step-by-Step Installation

### 1. Create the special repository

1. Go to **github.com → New repository**
2. Set the repository name to **your exact GitHub username**
3. Check **"Public"**
4. Check **"Add a README file"**
5. Click **Create repository**

### 2. Clone the repo locally

```bash
git clone https://github.com/asaad-cs/asaad-cs.git
cd asaad-cs
```

### 3. Copy the files from this folder

Copy these files into the cloned repo:

```
README.md           → root of the repo
assets/banner.svg   → assets/ folder inside the repo
```

The final repo structure should look like:

```
asaad-cs/
├── README.md
└── assets/
    └── banner.svg
```

### 4. Fill in the 5 placeholders

Open `README.md` and do a find-and-replace for each item:

| Placeholder | Replace with |
|---|---|
| `asaad-cs` | Your actual GitHub username (appears ~8 times) |
| `YOUR_LINKEDIN_HANDLE` | The handle at the end of your LinkedIn URL |
| `YOUR_PORTFOLIO_URL` | Your portfolio website URL |
| `YOUR_RFPILOT_REPO_NAME` | The exact name of your RFPilot repository |
| `YOUR_NASKH_REPO_NAME` | The exact name of your Naskh repository |

All URL-sensitive links are collected at the **bottom of README.md** under `LINK REFERENCES` — you only need to edit them in one place.

### 5. Push to GitHub

```bash
git add README.md assets/banner.svg
git commit -m "Add profile README"
git push origin main
```

Visit `github.com/asaad-cs` — the README renders automatically on your profile page.

---

## Widget Dependencies

All external widgets used are well-maintained open-source projects:

| Widget | Maintainer | Purpose |
|---|---|---|
| `github-readme-stats` | anuraghazra (4M+ stars) | GitHub stats card + Top Languages |
| `streak-stats.demolab.com` | DenverCoder1 | Contribution streak |
| `skillicons.dev` | tandpfun | Tech stack icons |
| `komarev.com/ghpvc` | antonkomarev | Profile view counter |
| `shields.io` | — (industry standard) | Status badges |

---

## Why Each Section Was Included

| Section | Reason |
|---|---|
| **Hero Banner** | First impression — your name and role in 2 seconds, before any text is read |
| **Profile Badges** | Quick-scan links for recruiters; profile views badge signals activity |
| **About Me** | Prose summary with 3 quantified achievements pulled directly from your CV; skimmable in 15 seconds |
| **Current Focus** | YAML block signals technical literacy and tells recruiters exactly what role you want |
| **Tech Stack** | Visual skill icons are faster to scan than bullet lists; grouped by domain so AI skills are seen first |
| **Featured Projects** | Ordered by technical impressiveness (RFPilot first for GPT-4o/RAG, Naskh second for hackathon impact, HRMS third for real delivery) |
| **GitHub Statistics** | Social proof — shows real commit history and language distribution |
| **Streak Stats** | Shows consistency and current coding activity |
| **Certifications** | Signals ongoing learning; AWS cert in progress shows ambition |
| **Connect** | Reduces friction for recruiters; one-click to all channels |
| **Footer** | Clean close with profile views counter and a soft CTA |

---

## Customization Tips

- **Profile photo**: GitHub automatically shows your avatar above the README — no action needed
- **Pinned repositories**: Pin RFPilot and Naskh on your profile page to complement the README cards
- **AWS cert**: Once you pass, change `🔄 In Progress` to `✅ Completed` and update the date
- **New projects**: Add them above the HRMS section as your portfolio grows
